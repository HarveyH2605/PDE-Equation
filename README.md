# PDE-Equation

This repository contains numerical implementations for solving various types of Partial Differential Equations (PDEs). The goal is to explore and analyze different methods by observing their accuracy, stability, and theoretical underpinnings. This includes parabolic, elliptic, and nonlinear PDEs with both explicit and implicit schemes.

---

## Contents

### Parabolic Equation

Numerical approaches to time-dependent PDEs (e.g., heat equation), where we discretize both time and space:

#### Forward Difference Method
- An explicit method.
- Simple to implement but conditionally stable.
- Used for equations like:  
  ∂u/∂t = α ∂²u/∂x²

#### Backward Difference Method
- An implicit method.
- Unconditionally stable but requires solving a linear system at each step.
- Good for stiff equations.

#### Crank-Nicolson Method
- A semi-implicit method that averages Forward and Backward methods.
- Second-order accurate in both time and space.
- Balance between stability and accuracy.

---

### Finite Difference Method for Elliptic Equation

Applies to steady-state PDEs (e.g., Laplace and Poisson equations). This section will:
- Discretize the spatial domain using central differences.
- Solve the resulting linear system iteratively (e.g., Gauss-Seidel, SOR) or directly.
- Example PDE:  
  ∂²u/∂x² + ∂²u/∂y² = f(x, y)

---

### Nonlinear PDE

Methods to solve nonlinear partial differential equations, particularly those involving implicit schemes.

#### Implicit Newton Method
- Solves nonlinear PDEs using Newton-Raphson iteration.
- Involves computing and inverting the Jacobian matrix.
- Applied to problems like nonlinear diffusion or reaction-diffusion equations.
