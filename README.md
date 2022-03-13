# Python implementation of Finite Element Method to solve Laplace equation

This generic code is presented with the following example:

![sys](https://latex.codecogs.com/gif.latex?%5Cbegin%7Bcases%7D%20%5C%3B%5C%3B%5Cnabla%5E2u%3D0%20%26%20%5C%3B%5C%3B%28x%2Cy%29%5Cin%280%2C1%29%5Ctimes%280%2C1%29%20%5C%5C%20%5C%3B%5C%3Bu%28x%2C0%29%3D%5Csin%28%5Cpi%20x%29%20%26%20%5C%3B%5C%3Bx%5Cin%5B0%2C1%5D%20%5C%5C%20%5C%3B%5C%3Bu%28x%2C1%29%3D0%20%26%20%5C%3B%5C%3Bx%5Cin%5B0%2C1%5D%20%5C%5C%20%5C%3B%5C%3Bu%280%2Cy%29%3Du%281%2Cy%29%3D0%20%26%20%5C%3B%5C%3By%5Cin%5B0%2C1%5D%20%5Cend%7Bcases%7D)

which has analytical solution:

![sol](https://latex.codecogs.com/gif.latex?u%28x%2Cy%29%3D%5Csin%28%5Cpi%20x%29%5B%5Ccosh%28%5Cpi%20y%29-%5Ccoth%28%5Cpi%29%5Csinh%28%5Cpi%20y%29%5D)

The distribution of files is as follows:

  * exampleFunctions.py : file containing Dirichlet boundary conditions function and analytical solution function
  * femFunctions.py : FEM architecture functions, including some additional plot functions (mesh and errors convergence)
  * FEM_2D.py : main file performing the assembly and solving the system, plots generation
