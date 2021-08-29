## Chapter1_Convexity

# Why is conveity important? 

For convex programming problems, and more particularly for linear programs, local solutions are also global solutions, which generally makes them easier to solve both in theory and practice. 

On the other hand, general nonlinear problems, both constrained and unconstrained, may possess local solutions that are not global solutions. 

# Definition: 

A function f is convex and a convex set S if it satisifies
f (ax + (1 − a)y) <= af (x) + (1 − a) f (y), for all a in [0, 1].

# Theorem (Global solutions of convex optimization): 
Let x* be a local minimizer of a convex optimization. Then, x* is also a global minimizer. If the objective function is strictly convex, then x* is the unique global minimizer. 

# Derivatives and Convexity:
It might be difficult to determine whether or not a function is convex using the definition. For a 1-D function f that has two contrinuous derivatives, there is an easier way:

### The function f is convex if f''(x) > 0, for all x in set S. ###

### In multi-demension case, the Hessian Matrix is positive semidefinite. ###

For every point x in set S, xT Hx,-2 f (x().
![image](https://user-images.githubusercontent.com/88390140/131263324-6617bdd9-0d74-4142-a1c2-7e27c38c5c9f.png)
