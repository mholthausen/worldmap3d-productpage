+++
fragment = "item"
weight = 20
background = "light"

+++
The viewer can be used to integrate data services that provide their information as a WMS/WMTS, WMS-Time, GeoJSON or CZML. Vector data stored as KML, GeoJSON, or CZML and small glTF files can be used as-is. Larger data sets must be converted into a supported format. All formats that can be interpreted by CesiumJS can also be integrated into WorldMap3D. These must be stored on a server and streamed into the application. These supported formats include Cesium 3D Tiles, Imagery, Terrain and glTF.

Go to [Data Types and Formats](https://cesium.com/learn/3d-tiling/tiler-data-formats/) for detailed information on supported formates and data types.

### HLOD

The tiles are organized in a tree structure that implements the concept of hierarchical level of detail (HLOD) for an optimal representation of spatial data. Here, each tile has a so-called bounding volume. This refers to an object that defines a spatial extent that completely encloses its contents. The content of all subordinate tiles is completely within the bounding volume of the parent tile.
