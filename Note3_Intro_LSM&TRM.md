## Resources Link
#### Line Search Method: https://optimization.mccormick.northwestern.edu/index.php/Line_search_methods     
#### Convergence of Algorithms: https://caam37830.github.io/book/01_analysis/convergence.html#:~:text=Many%20numerical%20algorithms%20converge%20to%20a%20solution%2C%20meaning,k%20%E2%86%92%20%E2%88%9E%20%CF%B5%20k%20%3D%200%20%24      
#### Algorithms and their convergence: http://macs.citadel.edu/chenm/343.dir/11.dir/lect1_3.pdf      
___________________________________________________________________________________________________________________________________________________________________________________

**Sometime, problem is so complex that made function/formula cannot be expressed generally and explicitly. Previous method, which find the first-derivative equal to 0, can not work.**     

## Review: 
General OP Algorithm: 
1. Specify some initial guess of the solution x_0.     
2. For k = 0, 1, ...     
    (1) If x_k is optimal, stop.     
    (2) Determine x_k+1, a new estimate of the solution.     

We choose x_k+1 given information about f at x_k (and possibly even earlier iterates) so that f(x_k+1) < f(x_k).     
To move frim x_k to x_k+1: Two Fundemental Strategies, **Line Search Method** and **Trust Region Method**.    

## Definition:    

 Line Search Strategy | Trust Region Strategy         
----------------------|-----------------------------------------
 Choose a direction p_k     |  Construct a model function m_k (typically, quadratic) that is similar to (but simpler than) f around x_k   
 Search along p_k from x_k to x_k+1 with f(x_k+1)<f(x_k).   |  Search for x_k+1 with m_k(x_k+1)<m_k(x_k) inside a small trust region (typically a ball) around x_k.      
 Approximately solve the 1-D minimization problem: g(a)=f(x_k+a* p_k). Minimize g(a) via a subject to a>=0.   |   Approximately solve the n-D minimization problem: minimize m_k(x_k + p) via p subject to x_k + p in trust region.
  ||  If x_k+1 does not produce enough decay in f, shrink the region.     

## Mathematical form:        
 -  Line Search Method:      
![image](https://user-images.githubusercontent.com/88390140/131764100-aa19cf9f-3a73-48bd-a747-3e5b06418faa.png)      
 -  Trust Region Method:          
![image](https://user-images.githubusercontent.com/88390140/131764954-f47d418f-e82e-4479-90af-1449da1302fd.png)


 Line Search Method | Trust Region Method    
---------------------|-----------------------------------------
 Fix direction     |  Fix maximum distance     
 Step legth        |  Choose direction and actual distance     
X_k = X_k + a * p_k |  X_k = X_k + p_k  

## Rates of Convergence 
Many of the algorithms do not find a solution in a finite number of steps. 
When discussing such an algorithm, the following two questions are often asked:
1. Does it converge?
2. How fast does it converge? *Focus*

