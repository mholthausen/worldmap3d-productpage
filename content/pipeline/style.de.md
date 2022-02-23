+++
fragment = "item"
weight = 20
background = "light"

+++
Neben bereits prozessierten 3D-Objekten kann über einen Importdienst innerhalb des Clients eine Möglichkeit zum Upload der 2D-Datensätze ermöglicht werden. Hierbei werden die Daten zunächst in einer PostGIS persistiert und in das erforderliche Koordinatensystem konvertiert. Anschließend wird über [py3dtiles](https://gitlab.com/Oslandia/py3dtiles) ein 3D Tiles aus den Daten generiert. Über eine Erweiterung werden diese dann zu einem 3D Tileset zusammengesetzt. Parallel können entsprechende Metadaten generiert werden. Anschließend steht das Objekt in dem Client wieder zur Verfügung.

![3D Import Pipeline](../../images/ablauf_importer.png)
