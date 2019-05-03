Copyright: Mohammad Safeea, May-2019
----------------------------------------
This folder contains the scripts for generating a MATLAB file (.m function) that can calculate the christoffel symbols of a specific robot.
The equations in the (.m function) are generated symbolically based on Lagrangian method.

The equations are generated only for the upper triangular part of Christoffel symbols, as to increase the efficiency of the generated equations.
-----------------------------------------
This folder includes:
1- a01_generateChristoffelSymbolicFunction.m: a MATLAB script used to generate the (.m function) of a specific robot.
2- generateRandomRobot.m: a MATLAB script used to generate a data structure for a serially linked robot.
3- GetKenimaticModelAccelerated.m: a MATLAB function used to calculate the transformation matrices of a robot based on its configurationa and DH paramenters.
4- Readme.txt: this file
5- robotStructure_5DOF.mat: data (mat file) of DH paramenters and inertial data of a 5DOF serially linked robot.
6- rotx.m,roty.m,rotz.m: MATLAB functions, used to calculate rotation matrices.
