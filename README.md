## Unsere Idee:
Ein beliebiges Bild des Users wird umgewandelt in eine ausdruckbare Vorlage für
3D Pixelart mit konkavem Tiefeneffekt, welche mit Bügelperlen gebaut werden kann.
Dabei hat der User die Freiheit, die Skalierung und Größe das Bilds anzupassen, sowie
die Anzahl und Verteilung der Layer frei zu verändern.
Wir liefern dafür die Tools zur Bearbeitung, eine Vorschau des Ergebnisses und eine
druckbare Anleitung zum selbst Bauen.
Die Anleitung beinhält dabei je eine Steckvorlage für die einzelnen Layer,
eine Anzahl an benötigten Bügelperlen und eine Anleitung zum Zusammenschmelzen der Layer.

![ActivityDiaBildVorschau](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/Karma-chocolate/SWE-Labor/refs/heads/main/ActivityDiaBildvorschau.puml?token=GHSAT0AAAAAADN4FNLONP2OVUTI62Q7YCIA2JAPZLA)

![ActivityDiaLayerAnpassen](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/Karma-chocolate/SWE-Labor/refs/heads/main/ActivityDiaLayerAnpassen.puml?token=GHSAT0AAAAAADN4FNLOEKXNAIDU3ZPABEAM2JAP7YA)
## Klassendiagramm
Die zentralen Konzepte unsere Anwendung konnten wir in 7 Entitäten zusammenfassen. Dabei steht der Nutzer natürlich als Verwender des Systems. Außerdem übergibt er das zu verwendende Bild und erhält am Ende die fertige Anleitung. Das System selbst verwendet für verschiedene Operationen den Colormapper und den Exporter und speichert alle Fortschritte im Projekt.
![ClassDiagramm](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/Karma-chocolate/SWE-Labor/refs/heads/main/ClassDiagramm.puml?token=GHSAT0AAAAAADN4FNLOVI3XOTQ56737GJ7K2JAP73Q)

## System-Sequenz-Diagramm
Zuerst lädt der User ein Bild hoch, welches dann vom System konvertiert und verarbeitet wird. Dazu werden Defaultwerte zur Umwandlung genutzt. Danach gibt das System eine Preview und ermöglicht ab jetzt dem Nutzer verschiedene Operationen. Zum einen kann er einzelne Farben manuell abändern, die Grenzen und Anzahl der Layer anpassen und die allgemeine Größe und das Format anpassen. Nachdem der User seine Anpassungen vorgenommen hat, kann er zuletzt eine Anleitung anfordern.
![SystemSequenzDia](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/Karma-chocolate/SWE-Labor/refs/heads/main/System-Sequenz-Diagramm.puml?token=GHSAT0AAAAAADN4FNLO236YPVUWRAHQI46Y2JARJSA)
![Vorlage](http://www.plantuml.com/plantuml/proxy?cache=no&src="hierRawLink")
