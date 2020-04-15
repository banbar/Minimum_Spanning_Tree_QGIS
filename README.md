# "Minimum Spanning Tree" Plugin @ QGIS 3

This repository contains the sample data and code of the "Minimum Spanning Tree" plugin of QGIS 3. The plugin can be downloaded from: https://plugins.qgis.org/plugins/minimum_spanning_tree/

<img src="images/gui.jpg" width=350 align="center">

The plugin identifies the Minimum Spanning Tree (MST) of geographical inputs. Three different ways to determine costs of edges are considered, which constitute the tabs of the plugin: 
1. **Vector**: Provided by the given input linestring. 
2. **Automatic**: Obtained automatically based on the input shapefile. Delaunay Triangulation is used to obtain the edges, and Euclidean distance is used to determine the costs. 
3. **Raster**: Both raster and vector data are used to estimate the costs of edges. In all of the cost estimation methods, there is an optional barrier (obstacle) input, which makes sure that no edge in MST intersects with a barrier provided as a linestring. To obtain reliable results, all of the inputs must be in the same coordinate system.

<img src="images/flowchart.jpg" width = 700 align="center">


