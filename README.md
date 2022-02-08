# ENM_TP

Welcome to the directory dedicated to the different python tutorials done in class.
Only the python labs are here, the ones done in other languages (Matlab, Java, R, Fortran) will be converted soon.

- [TP_40andmore_dimensional_equations_RK4](#TP-40andmore-dimensional-equations-RK4)
- [TP_HeatEquation](#TP-HeatEquation)
- [TP_Optimisation_GaussNewton](#TP-Optimisation-GaussNewton)

## TP 40andmore dimensional equations RK4
The objective of this notebook is to explore the notion of numerical solution of an ordinary derivative equation or a system of such equations.
The work starts with a simple example, the harmonic oscillator, which allows to recall elementary notions on dynamical systems. A physical analysis, then a mathematical one, allows to understand the dynamics and to introduce the numerical resolution. In particular, a first calculation code is proposed for the resolution of this dynamics. This example illustrates the conversion of an ordinary differential equation to a first order differential equation system.
For the harmonic oscillator, the numerical solution is not relevant since simple analytical solutions exist. We are then interested in another model problem: the non-linear oscillator, for which there is no simple solution. Numerical exploration allows us to characterise the properties of the trajectories that may be difficult to characterise analytically.
These two oscillators illustrate dynamics in a space of dimension 2 . However, in the problems encountered in meteorology, the dimension of the spaces manipulated can be greater than 109 . In order to be aware of problems in higher dimension, a model of intermediate dimension, 40 is introduced, this number of dimension being able to be modified at will.

## TP HeatEquation

We wish to solve the heat problem with the following homogeneous Dirichlet boundary conditions:
$$ (P)~ \left \{
        \begin{array}{11}
            \ \displaystyle \frac{\partial u}{\partial t}-\Delta u = f \, \, \, \, \, \, (\Omega \times [0, T])\\
            \ u(0,t)=0 \, \, \, \, \, \, (\partial \Omega) \\
            \ u(1,t)=0 \, \, \, \, \, \, (\partial \Omega) \\
            \ u(x,0)=u_{0}(x) \, \, \, \, \, \, (t=0)
         \end{array} 
         \right. $$
   on a one-dimensional domain Ω by a finite difference discretization method. We propose to detail step by step the different steps by systematically performing unit tests in order to validate your implementations.
The proposed steps are the following:

Impose an exact solution 𝑢𝑒𝑥(𝑥,𝑡) to problem (𝑃) .
Deduce an initial condition 𝑢0(𝑥) to problem (𝑃) .
Deduce 𝑓 the source term associated with 𝑢𝑒𝑥(𝑥,𝑡) .
Solve numerically (𝑃) using the explicit and implicit Euler schemes.
Determine numerically the order of convergence of the time discretization schemes.

## TP Optimisation GaussNewton
The objective is to program the Gauss-Newton methods for a least squares problem
$$
({\cal P})\left\{ 
\begin{array}{l}
Min\;\;f(\beta)=(1/2)||r(\beta)||^2 \\ 
\beta \in \mathbb{R}^p
\end{array}
\right. 
$$
where $r$ is the residual function
$$ 
\begin{array}{cc}
    r:\mathbb{R}^p  & \rightarrow & {\mathbb{R}^n} \\
            {\beta} & \rightarrow & r(\beta).
 \end{array}
 $$
 
 The objective is to use a generic code for the Gauss-Newton algorithm and for the Newton algorithm for solving the least squares problem.
 
