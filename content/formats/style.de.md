+++
fragment = "item"
weight = 20
background = "light"

+++
Der Viewer kann verwendet werden, um Datendienste zu integrieren, die ihre Informationen als WMS/WMTS, WMS-Time, GeoJSON oder CZML bereitstellen. Als KML, GeoJSON oder CZML gespeicherte Vektordaten und kleine glTF-Dateien können unverändert verwendet werden. Größere Datensätze müssen in ein unterstütztes Format konvertiert werden. Alle Formate, die von CesiumJS interpretiert werden können, können auch in WorldMap3D integriert werden. Diese müssen auf einem Server gespeichert sein und in die Anwendung gestreamt werden. Zu den unterstützten Formaten gehören Cesium 3D Tiles, Imagery, Terrain und glTF.

Ausführliche Informationen zu den unterstützten Formaten und Datentypen finden Sie unter [Datentypen und -formate](https://cesium.com/learn/3d-tiling/tiler-data-formats/).

### HLOD

Die Kacheln sind in einer Baumstruktur organisiert, die das Konzept der hierarchischen Detailebene (HLOD) für eine optimale Darstellung von räumlichen Daten beinhaltet. Jede Kachel hat ein Begrenzungsvolumen, ein Objekt, das eine räumliche Ausdehnung definiert, die ihren Inhalt vollständig umschließt. Der Baum ist räumlich kohärent; der Inhalt der untergeordneten Kacheln befindet sich vollständig innerhalb des Begrenzungsvolumens der übergeordneten Kachel.
