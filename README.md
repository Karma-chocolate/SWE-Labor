## Unsere Idee:
Ein beliebiges Bild des Users wird umgewandelt in eine ausdruckbare Vorlage für
3D Pixelart mit konkavem Tiefeneffekt, welche mit Bügelperlen gebaut werden kann.
Dabei hat der User die Freiheit, die Skalierung und Größe das Bilds anzupassen, sowie
die Anzahl und Verteilung der Layer frei zu verändern.
Wir liefern dafür die Tools zur Bearbeitung, eine Vorschau des Ergebnisses und eine
druckbare Anleitung zum selbst Bauen.
Die Anleitung beinhält dabei je eine Steckvorlage für die einzelnen Layer,
eine Anzahl an benötigten Bügelperlen und eine Anleitung zum Zusammenschmelzen der Layer.



## Activity-Diagramm "Layer anpassen"
![ActivityDiaLayerAnpassen](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/Karma-chocolate/SWE-Labor/main/ActivityDiaBildvorschau.puml)

## Activity-Diagramm "Preview ansehen"
![ActivityDiaBildVorschau](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/Karma-chocolate/SWE-Labor/main/ActivityDiaLayerAnpassen.puml)

## Use Cases

| Beschreibung                                                     | Name  | Prio | Status | Fragen | Req. |
| ---------------------------------------------------------------- | ---------------------- | ---- | ------ | ------ | ---- |
| Nutzer lädt Bild hoch und kann ersten Draft ansehen              | Bildvorschau ansehen   | essenziell    | offen      | –      | 22, 44, 51    |
| Dimension des Perlenrasters festlegen                            | Dimensionen festlegen  | wichtig    | offen      | –      | 33, 44    |
| Manuelle Layeranpassung durch Nutzer, wieviele und ab wo Grenzen | Layer anpassen         | unwichtig    | offen      | –      | 52    |
| Export des Projekts in .pdf oder .png                            | Export                 | essenziell    | offen      | –      | 11    |
| Nutzer speichert das Projekt ab                                  | Projekt speichern      | wichtig    | offen      | –      | 51    |

## Begründungen für Prioritäten

- Der Nutzer braucht eine Vorschau, um einzuschätzen ob das Ergebnis den Erwartungen entspricht, beveor es gedruckt wird.
- Um individuelle Ergebnisse zu bekommen, müssen die Dimensionen anpassbar sein.
- Die layeranpassung ist gut für spezielle Anforderungen, aber nicht relevant um ein gutes Ergebniss zu bekommen.
- Damit das Programm seinen zweck erfüllt, muss der Nutzer das Projekt drucken können.
- Um alte Projekte nicht von neu aufbauen zu müssen, ist es sinnvoll alte Projekt speichern und wieder öffnen zu können.

## Use-Case-diagramm
![Use-Case](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/Karma-chocolate/SWE-Labor/main/UseCaseUML.puml)

## Klassendiagramm
Die zentralen Konzepte unsere Anwendung konnten wir in 7 Entitäten zusammenfassen. Dabei steht der Nutzer natürlich als Verwender des Systems. Außerdem übergibt er das zu verwendende Bild und erhält am Ende die fertige Anleitung. Das System selbst verwendet für verschiedene Operationen den Colormapper und den Exporter und speichert alle Fortschritte im Projekt.

![ClassDiagramm](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/Karma-chocolate/SWE-Labor/main/ClassDiagramm.puml)

## System-Sequenz-Diagramm
Zuerst lädt der User ein Bild hoch, welches dann vom System konvertiert und verarbeitet wird. Dazu werden Defaultwerte zur Umwandlung genutzt. Danach gibt das System eine Preview und ermöglicht ab jetzt dem Nutzer verschiedene Operationen. Zum einen kann er einzelne Farben manuell abändern, die Grenzen und Anzahl der Layer anpassen und die allgemeine Größe und das Format anpassen. Nachdem der User seine Anpassungen vorgenommen hat, kann er zuletzt eine Anleitung anfordern.

![SystemSequenzDia](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/Karma-chocolate/SWE-Labor/main/System-Sequenz-Diagramm.puml)

## Anforderungen

| ID | Nr. | Kategorie | Name                         | Beschreibung                                                                                                                              | Prio | Status | Messwert              
| -- | --- | --------- | ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ---- | ------ | ------------------- |
| 1  | 1   | fct       | Anleitung                    | Eine 1:1 Abbildung der zu legenden Bügelperlen. Jeweils eine Abbildung pro Layer und eine Anleitung zum Zusammenfügen der Ebenen im Ofen. | high | open   | –                   |
| 2  | 2   | fct       | Kompatibilität des Inputs    | Unterstützung verschiedener Bildgrößen und Bildtypen (JPG, PNG, BMP).                                                                     | med  | open   | –                   |
| 3  | 3   | fct       | Variabler Output             | Modulare Größe des Ergebnisses und der Anleitung dazu.                                                                                    | low  | open   | –                   |
| 4  | 4   | fct       | Komprimierung und Skalierung | Das Komprimieren der Farben sowie das Downsizing des Bildes auf die gewünschte Bildgröße.                                                 | high | open   | –                   |
| 5  | 1   | non fct   | UI                           | Verständliches, übersichtliches und benutzerfreundliches UI                                                                               | med  | open   | kundenzufriedenheit |
| 6  | 2   | non fct   | Layering                     | Das Bügelperlenbild erhält einen 3D-Layering-Effekt durch das Hinzufügen mehrerer Ebenen                                                  | med  | open   | kundenzufriedenheit |

## Verwendung von LLMS:
Wir haben für diese Präsentation LLMS (ChatGPT) für die erstellung von Plant UML Diagrammen verwendet.

![Vorlage](http://www.plantuml.com/plantuml/proxy?cache=no&src="hierRawLink")
