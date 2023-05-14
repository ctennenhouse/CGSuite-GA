# CGSuite-GA
Genetic Algorithm written for CG Suite 2.x

CG Suite 2.0 is much more powerful and extendible than previous versions. It is, however, missing some tools that would be helpful for applying stochastic methods to combinatorial game analyses. I wrote this code to search for high temperature positions in DOmineering by way of Partizan Arc Kayles. Note that the code for PAK itself is not currently included here.

This code uses lots of global variables in order to continue a previous run of the algorithm. It also requires a random seed, since there is currently no way to access the clock or any other external data to seed the (very simple) pseudo-random number generator. Hopefully there are sufficient comments to understand how to run and modify this code. Obviously CG Suite 2.x is required, as is the Partizan Arc Kayles CG Script file. The mechanics of the algorithm and its associated routines should be modifiable to other applications.

This file should go in the CGScript folder, along with startup.cgs. Initiate it by running ga_trees_x() in the worksheet. Don't forget to set the seed.

Notes:
  CGs like dyadic rationals, and this is reflected in the PRN generator. So don't expect random() to return anything uniform. But it does the job.
  
