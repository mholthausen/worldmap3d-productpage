+++
fragment = "item"
weight = 20
background = "light"

+++
In addition to already processed 3D objects, an import service within the client can enable a possibility to upload 2D datasets. Here, the data is first persisted in a PostGIS and converted into the required coordinate system. Subsequently, a 3D tile is generated from the data via [py3dtiles](https://gitlab.com/Oslandia/py3dtiles). Via an extension these are then assembled to a 3D tileset. In parallel, appropriate metadata can be generated. Afterwards the object is available as 3D in the client again.

![3D Import Pipeline](../../images/ablauf_importer.png)