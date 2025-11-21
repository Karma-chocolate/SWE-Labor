@startuml
title Kombiniertes Activity-Diagramm (Use Case 1 + 2)

|Nutzer|
start
:Startet Anwendung;

|System|
:Initialisiert Anwendung;
if (Gespeichertes Projekt vorhanden?) then (Ja)
  :Lädt letztes Projekt;
else (Nein)
  :Erstellt neues Default-Projekt;
endif
:Zeigt Defaultscreen;

|Nutzer|
:Importiert Bild;

|System|
:Skaliert Originalbild;
:Berechnet Average-Farben / beste Näherungsfarben;
:Erstellt Default-Layer;
:Zeigt erste Vorschau;

|Nutzer|
:Passt Layeranzahl an;
:Wählt Grenzen & Dimensionen der Layer;
:Drückt "Vorschau erstellen";

|System|
:Erstellt neue Vorschau;
:Zeigt aktualisierte Vorschau;

|Nutzer|
stop
@enduml 

