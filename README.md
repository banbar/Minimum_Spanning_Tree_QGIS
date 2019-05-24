# "Minimum Spanning Tree" Plugin of QGIS3
This repository is the experimental plugin entitled "Minimum Spanning Tree" of QGIS 3.

This plugin finds the Minimum Spanning Tree (MST) of an input polygon shp file using Kruskal's algorithm. 

First, the centroids of the polygons are determined and those adjacent polygons are connected through an edge. The cost of an edge is the distance between the centroids. Second, Kruskal's algorithm is executed to determine the MST. The centroids, edges and the resulting MST are all added as a virtual layer.

Given the following examplar input of Turkish districts, the output is as follows: 
- - - -


![MST of districts](https://pbs.twimg.com/media/Dz--HO9X0AEYTZn.jpg:large)




