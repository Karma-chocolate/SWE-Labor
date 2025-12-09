## 1. 3D Perlenbild [ brsi1022 / doal1018 / plni1012 ]

![Beispiel](https://github.com/Karma-chocolate/SWE-Labor/blob/main/evoli.jpg?raw=true)
Ein beliebiges Bild des Users wird umgewandelt in eine ausdruckbare Vorlage für
3D Pixelart mit konkavem Tiefeneffekt, welche mit Bügelperlen gebaut werden kann.
Dabei hat der User die Freiheit, die Skalierung und Größe des Bilds anzupassen, sowie
die Anzahl und Verteilung der Layer frei zu verändern.
Wir liefern dafür die Tools zur Bearbeitung, eine Vorschau des Ergebnisses und eine
ausdruckbare Anleitung zum selbst Bauen.
Die Anleitung beinhält dabei je eine Steckvorlage pro Layer,
eine Anzahl an benötigten Bügelperlen und eine Anleitung zum Zusammenschmelzen der Layer.


## 2. Use Cases
![Use-Case](https://github.com/Karma-chocolate/SWE-Labor/blob/main/UseCaseDia.png?raw=true)

| Beschreibung                                                     | Name  | Prio | Status | Fragen | Req. |
| ---------------------------------------------------------------- | ---------------------- | ---- | ------ | ------ | ---- |
| Nutzer lädt Bild hoch und kann ersten Draft ansehen              | Bildvorschau ansehen   | essenziell    | offen      | –      | 22, 44, 51    |
| Nutzer legt die Dimensionen des Perlenrasters fest               | Dimensionen festlegen  | wichtig    | offen      | –      | 33, 44    |
| Nutzer passt Anzahl und Grenzen der Layer an                     | Layer anpassen         | unwichtig    | offen      | –      | 52    |
| Nutzer exportiert das Projekt in .pdf oder .png                  | Export                 | essenziell    | offen      | –      | 11    |
| Nutzer speichert das Projekt ab                                  | Projekt speichern      | wichtig    | offen      | –      | 51    |

## 3. Begründungen für Prioritäten

- Der Nutzer braucht eine Vorschau, um Einzuschätzen ob das Ergebnis den Erwartungen entspricht bevor es gedruckt wird.
- Anpassbare Dimensionen machen das Ergebniss individualisierbar und bieten auch die Möglichkeit zur Begrenzung des benötigten Materials.
- Layeranpassungen sind praktisch für spezielle Anforderungen, aber nicht relevant um ein gutes Ergebniss zu bekommen.
- Damit das Programm seinen Zweck erfüllen kann, muss der Nutzer das Projekt drucken können.
- Um Projekte nicht von neu aufbauen zu müssen, ist es sinnvoll alte Projekt speichern und wieder öffnen zu können.

## 4. Anforderungen

| ID | Nr. | Kategorie | Name                         | Beschreibung                                                                                                                              | Prio | Status | Messwert              
| -- | --- | --------- | ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ---- | ------ | ------------------- |
| 1  | 1   | fct       | Anleitung                    | Eine 1:1 Abbildung der zu legenden Bügelperlen. Jeweils eine Abbildung pro Layer und eine Anleitung zum Zusammenfügen der Ebenen im Ofen. | high | open   | –                   |
| 2  | 2   | fct       | Kompatibilität des Inputs    | Unterstützung verschiedener Bildgrößen und Bildtypen (JPG, PNG, BMP).                                                                     | med  | open   | –                   |
| 3  | 3   | fct       | Variabler Output             | Modulare Größe des Ergebnisses und der Anleitung dazu.                                                                                    | low  | open   | –                   |
| 4  | 4   | fct       | Komprimierung und Skalierung | Das Komprimieren der Farben sowie das Downsizing des Bildes auf die gewünschte Bildgröße.                                                 | high | open   | –                   |
| 5  | 1   | non fct   | UI                           | Verständliches, übersichtliches und benutzerfreundliches UI                                                                               | med  | open   | kundenzufriedenheit |
| 6  | 2   | non fct   | Layering                     | Das Bügelperlenbild erhält einen 3D-Layering-Effekt durch das Hinzufügen mehrerer Ebenen                                                  | med  | open   | kundenzufriedenheit |


## 5. Activity-Diagramm "Preview ansehen"
![ActivityDiaBildVorschau](https://github.com/Karma-chocolate/SWE-Labor/blob/main/activityDia.png?raw=true)

## 6. Activity-Diagramm "Layer anpassen"
![ActivityDiaLayerAnpassen](https://github.com/Karma-chocolate/SWE-Labor/blob/main/?raw=true)

## 7. Klassendiagramm
Die zentralen Konzepte unsere Anwendung konnten wir in 7 Entitäten zusammenfassen. Dabei steht der Nutzer natürlich als außenstehender Verwender des Systems. Außerdem übergibt er das zu verwendende Bild und erhält am Ende die vom System erstellte Anleitung. Das System verwendet für das Anpassen und Erstellen einer Anleitung den Colormapper und den Exporter und speichert alle Fortschritte im Projekt.
![ClassDiagramm](https://github.com/Karma-chocolate/SWE-Labor/blob/main/classDia.png?raw=true)

## 8. System-Sequenz-Diagramm
Zuerst lädt der Nutzer ein Bild hoch, welches dann vom System konvertiert und verarbeitet wird. Dazu werden Defaultwerte zur Umwandlung genutzt. Danach gibt das System eine Preview und ermöglicht ab jetzt dem Nutzer verschiedene Operationen. Zum einen kann er einzelne Farben manuell abändern, die Grenzen und Anzahl der Layer anpassen und die allgemeine Größe und das Format anpassen. Nachdem der Nutzer seine Anpassungen vorgenommen hat, kann er zuletzt eine Anleitung generieren.
![SystemSequenzDia](https://github.com/Karma-chocolate/SWE-Labor/blob/main/sequenzDia.png?raw=true)

## Verwendung von LLMS:
Wir haben für diese Präsentation LLMs (ChatGPT) für die Erstellung von Plant UML Diagrammen verwendet.

![Vorlage](http://www.plantuml.com/plantuml/proxy?cache=no&src="hierRawLink")
