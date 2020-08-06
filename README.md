# Minimum Spanning Tree Plugin @ QGIS 3

This repository contains the sample data and code of the 'Minimum Spanning Tree' plugin of QGIS 3.x. 
* The plugin can be downloaded from: <a href="https://plugins.qgis.org/plugins/minimum_spanning_tree" target="_blank">`https://plugins.qgis.org/plugins/minimum_spanning_tree`</a> 
* Video tutorial: <a href="https://www.youtube.com/watch?v=Tcdvlk_NS8w&feature=youtu.be" target="_blank">`https://www.youtube.com/watch?v=Tcdvlk_NS8w&feature=youtu.be`</a>  

**Citation:** If you are using this plugin for scientific research, please cite the paper <a href=https://www.sciencedirect.com/science/article/pii/S2352711020301771>`<b>Geo-MST: A geographical minimum spanning tree plugin for QGIS</b></a> 

<p align="center">
  <img width="350" src="images/gui.jpg">
</p>


The plugin identifies the Minimum Spanning Tree (MST) of geographical inputs. Three different ways to determine costs of edges are considered, which constitute the tabs of the plugin: 
1. **Vector**: Provided by the given input linestring. 
2. **Automatic**: Obtained automatically based on the input shapefile. Delaunay Triangulation is used to obtain the edges, and Euclidean distance is used to determine the costs. 
3. **Raster**: Both raster and vector data are used to estimate the costs of edges. In all of the cost estimation methods, there is an optional barrier (obstacle) input, which makes sure that no edge in MST intersects with a barrier provided as a linestring. To obtain reliable results, all of the inputs must be in the same coordinate system.

Raster data can be downloaded from: <a href="http://yunus.hacettepe.edu.tr/~banbar/mst_raster.zip" target="_blank">`http://yunus.hacettepe.edu.tr/~banbar/mst_raster.zip`</a>

<p align="center">
  <img width="600" src="images/flowchart.jpg">
</p>

The OSGeo functionalities used within the plugin are described [here](https://raw.githubusercontent.com/banbar/Minimum_Spanning_Tree_QGIS/431cf56ff2e6bc088d7adceac0c8923f849cfd11/img/code%20diagram_explanations.svg).
