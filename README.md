# ant_cube
ant cube problem from \<redacted company\> interview

## problem
Say you have an ant on a cube. The ant is doing a random walk on the edges of the cube, and every time it gets to a vertex it can choose which of the three edges it wants to go on (it can go back the way it came) with equal probability (1/3). Starting at some vertex, what is the expected number of steps/edge lengths the ant will walk before it comes back to the same vertex?

## analysis
Analysis was done in a Jupyter notebook (see above file) with simulation and in Octave with row reduction. The output of running the ant_cube.m file is given in a `.txt` file above. The method used in the Octave code was the ["first step"](http://www.maths.qmul.ac.uk/~ig/MAS338/FSAnalysis.pdf) method. 

Answer: the ant will take, on average, 8 steps to get back to its original position. We can see this from the simulation results in the Jupyter notebook but also from the results of the Octave code -- the first entry in the resulting vector corresponds to the expected number of steps before the ant returns to vertex 0 (the starting vertex). 
