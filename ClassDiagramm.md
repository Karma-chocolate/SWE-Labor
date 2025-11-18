@startuml
' --- Klassen ---
class System
class Nutzer
class Projekt
class Bild
class ColorMapper
class Exporter
class Anleitung

' --- Beziehungen ---

' Nutzer interagiert mit System
Nutzer --> System : verwendet

' Nutzer lädt Bild hoch
Nutzer --> Bild : lädt hoch

' Programm erstellt und verwaltet Projekte
System --> Projekt : verwaltet

' Projekt enthält ein Bild
Projekt --> Bild : enthält

' Programm verwendet ColorMapper zur\nBildverarbeitung
System --> ColorMapper : nutzt

' ColorMapper verarbeitet das Bild
ColorMapper --> Bild : verarbeitet

' Programm erzeugt Anleitung über Projekt
System --> Anleitung : erzeugt

' Exporter exportiert die erzeugte Anleitung
Exporter --> Anleitung : exportiert

' Programm nutzt Exporter für den Exportvorgang
System --> Exporter : nutzt

' Exporter nutzt Bild für den Exportvorgang
Exporter --> Bild : nutzt

' Programm nutzt Exporter für den Exportvorgang
Nutzer --> Anleitung : druckt
@enduml 

