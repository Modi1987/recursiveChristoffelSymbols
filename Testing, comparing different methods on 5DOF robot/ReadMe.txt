CopyRight: Mohammad Safeea, April-2019:
---------------------------------------
The following folder contains MATLAB functions for comparing 
the performance between both the:
1- Symbolic function for calculating the Christoffel Symbols
2- Recursive Numerical method for calculating the same.
--------------------------------------------------------------------------
The comparison is in terms:
1- Execution time: proposed method (numerical) is an order of magnitude faster than the symbolic
2- Function size: 760 KBytes with symbolic equation optimization, and 67MBytes without optimization
                             as compared to 4KBytes for the proposed algorithm.
3- Precission in calculation: Both methods give a comparable results, O(e-14) numerical difference in results.
4- Offline phase: the generation of the Symbolic function (christoffel_symbolicallyGenerated5dof.m) requires an offline phase, 
   it was generated using MATLAB R2018a, it took 8 days on a Intel i7 @3.6 GHz PC with 32GB RAM and Windows 10 OS.  
   Recursive Function does not require an offline phase. 
---------------------------------------------------------------------------
Included files:
1- a00_evaluate_comparison_test.m: MATLAB function used to run the comparison test.
2- christoffelNumerically.m: MATLAB function implementing proposed recursive method for calculating the Christoffel symbols.
3- GetKenimaticModelAccelerated.m: MATLAB function used for calculating the forward Kinematics.
4- ReadMe.txt: this file.
5- robotStructure_5DOF.mat: a MAT file containing the inertial data and the DH data of the manipulator used for comparison.
6- christoffel_symbolicallyGenerated5dof.m: is an offline generated MATLAB function, this function was generated using the Symbolic toolbox, it calculates
   the Christoffel symbols of a manipulator with DH & Inertial data that are defined in the mat file (robotStructure_5DOF.mat) 
7- test_results_5 DOF, execution time, 100 000 iterations.png: a print screen showing the results for comparing the execution time on the mentioned PC.
8- test_results_time to generating Symboic equations 5DOF.png: a print screen showing the time required to generate the Christoffel symbols function (christoffel_symbolicallyGenerated5dof.m) 
   symbolically using MATLAB R2018a on the mentioned PC.
---------------------------------------------------------------------------
To run the test, simply from MATLAB run the script (a00_evaluate_comparison_test.m)


Cheers!