# 2D_Geometry
Software allowing to create 2D geometries with different layers and discontinuities (faults and fractures) 

1- Change the parameters in the in-file ("name.dat"). Example given: "ing_7l_4f_big5.dat"

line 1-2: names of 2 output files (ex: oug.dat and out.dat);
line 3: number of nodes in the horizontal, nx, and vertical, ny, direction;
line 4: number of different soil types/layers;
line 5: number of coordinates given for layer 1 (n);
lines 6-5+n: coordnates of layer 1;
Then repeat for each layer;
line 117: number of discontinuities;
line 119: number of coordinates for discontinuity 1;
line 120-119+n: coordinates of discontinuity 1;
Then repeat for each discontinuity;

2- run 2D_Geometry.exe

enter the input file name ("name.dat")

3- plot the results using a software like grapher. The results are presented as groups of lines. Each group corresponds to a particular time of calculation. The last group corresponds to the final calculation stage.

"oug.dat"
column 1: x coordinate;
column 2: y coordinate;
column 3: x distance (m);
column 4: y distance (m);
column 5: layer number. "100" is for discontinuities;

"out.dat"
same minus column 5.