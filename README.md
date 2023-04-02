# Numerical solution of Schrodinger equation

## Time independent Schrodinger equation

The time-independent Schrödinger equation can be written as this eigenequation
$$\left[-\frac{\hbar^2}{2m}\frac{d^2}{dx^2} + V(x)\right]\psi(x) = E\psi(x)$$

The **shooting method** is a numerical approach used to solve the time-independent Schrödinger equation. In this method, the problem is reduced to finding the values of the energy parameter for which the solution satisfies a set of boundary conditions. This is achieved by guessing an initial value for the energy parameter and solving the differential equation using a numerical integration algorithm, such as the *Numerov propagator*. The solution is then checked against the boundary conditions, and the energy parameter is adjusted until the desired boundary conditions are satisfied. This process is repeated until convergence is achieved, and the final solution corresponds to the eigenvalue and eigenfunction of the Schrödinger equation.

The **Numerov propagator** is a fourth-order numerical integration algorithm that is particularly well-suited for solving second-order differential equations, such as the Schrödinger equation. It works by propagating the wave function through small steps in space, using a weighted average of the wave function at neighboring points to approximate the second derivative. This approach provides an accurate and efficient way to solve the Schrödinger equation and is widely used in quantum mechanics and other fields. The update rule used was
$$y_i = \frac{(10h^2(-2(E-c_{i-1})+24)y_{i-1}+(-2(E-c_{i-2})h^2-12)y_{i-2})}{12+2(E-c_i)h^2}$$
where $y$ is the $\Psi$ vector and $c$ stores the different potentials. 

<p align="center">
  <img src="images\image1.png" width="30%">
  <img src="images\image2.png" width="30%">
  <img src="images\image3.png" width="30%">
</p>

## Time dependent Schrodinger equation 

__ to do __
