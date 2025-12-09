## 1. Requirements

| ID | Nr. | Kategorie | Name                         | Beschreibung                                                                                                                              | Prio | Status | Messwert              
| -- | --- | --------- | ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ---- | ------ | ------------------- |
| 1  | 1   | fct       | Anleitung                    | Eine 1:1 Abbildung der zu legenden Bügelperlen. Jeweils eine Abbildung pro Layer und eine Anleitung zum Zusammenfügen der Ebenen im Ofen. | high | open   | –                   |
| 2  | 2   | fct       | Kompatibilität des Inputs    | Unterstützung verschiedener Bildgrößen und Bildtypen (JPG, PNG, BMP).                                                                     | med  | open   | –                   |
| 3  | 3   | fct       | Variabler Output             | Modulare Größe des Ergebnisses und der Anleitung dazu.                                                                                    | low  | open   | –                   |
| 4  | 4   | fct       | Komprimierung und Skalierung | Das Komprimieren der Farben sowie das Downsizing des Bildes auf die gewünschte Bildgröße.                                                 | high | open   | –                   |
| 5  | 1   | non fct   | UI                           | Verständliches, übersichtliches und benutzerfreundliches UI                                                                               | med  | open   | kundenzufriedenheit |
| 6  | 2   | non fct   | Layering                     | Das Bügelperlenbild erhält einen 3D-Layering-Effekt durch das Hinzufügen mehrerer Ebenen                                                  | med  | open   | kundenzufriedenheit |

## 2. Use Cases
![Use-Case](https://github.com/Karma-chocolate/SWE-Labor/blob/main/UseCaseDiagramm.png?raw=true)

| Beschreibung                                                     | Name  | Prio | Status | Fragen | Req. |
| ---------------------------------------------------------------- | ---------------------- | ---- | ------ | ------ | ---- |
| Nutzer lädt Bild hoch und kann ersten Draft ansehen              | Bildvorschau ansehen   | essenziell    | offen      | –      | 22, 44, 51    |
| Nutzer legt die Dimensionen des Perlenrasters fest               | Dimensionen festlegen  | wichtig    | offen      | –      | 33, 44    |
| Nutzer passt Anzahl und Grenzen der Layer an                     | Layer anpassen         | unwichtig    | offen      | –      | 52    |
| Nutzer exportiert das Projekt in .pdf oder .png                  | Export                 | essenziell    | offen      | –      | 11    |
| Nutzer speichert das Projekt ab                                  | Projekt speichern      | wichtig    | offen      | –      | 51    |

## 3. Activity-Diagramm "Preview ansehen"
![ActivityDiaBildVorschau](https://github.com/Karma-chocolate/SWE-Labor/blob/main/ActivitaetsDiagramm.png?raw=true)

## 4. Activity-Diagramm "Layer anpassen"
![ActivityDiaLayerAnpassen](https://github.com/Karma-chocolate/SWE-Labor/blob/main/plantumldia.png?raw=true)

## 5. Klassendiagramm
![ClassDiagramm](https://github.com/Karma-chocolate/SWE-Labor/blob/main/KlassenDiagramm.png?raw=true)

## 6. System-Sequenz-Diagramm
![SystemSequenzDia](https://github.com/Karma-chocolate/SWE-Labor/blob/main/SystemSeuenzDiagramm.png?raw=true)
