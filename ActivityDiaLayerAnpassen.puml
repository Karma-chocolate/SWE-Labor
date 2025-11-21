@startuml
title Activity Diagramm – Bild importieren, Vorschau vergrößern, Projekt speichern

|Nutzer|
start
:Startet die Anwendung;

|Maschine|
:Lädt letztes Projekt;
note right
Falls kein Projekt existiert, wird ein komplett neues
Default-Projekt geladen.
end note
:Zeigt Defaultscreen;

|Nutzer|
:Importiert ein Bild;

|Maschine|
:Skaliert Originalbild auf neue Größe;
:Nimmt Average der Farben für Downscale;
:Erstellt Layer nach Default-Einstellungen;
:Zeigt erste Vorschau der Vorlage;

|Nutzer|
:Sieht Vorschau und beschließt, das Bild zu vergrößern;
:Drückt "Vorschau erstellen";

|Maschine|
:Nimmt Average der Farben des Originalbilds
um beste skalierten Farben im neuen Format zu erzeugen;
:Zeigt neue Vorschau der Vorlage;

|Nutzer|
:Speichert Projekt ab;
stop

@enduml
