## References Link
Line Search Method: https://optimization.mccormick.northwestern.edu/index.php/Line_search_methods     
Root-footing: http://www.cas.mcmaster.ca/~cs4te3/notes/LineSearchMethods.pdf     
Convergence of Algorithms: https://caam37830.github.io/book/01_analysis/convergence.html#:~:text=Many%20numerical%20algorithms%20converge%20to%20a%20solution%2C%20meaning,k%20%E2%86%92%20%E2%88%9E%20%CF%B5%20k%20%3D%200%20%24      
Algorithms and their convergence: http://macs.citadel.edu/chenm/343.dir/11.dir/lect1_3.pdf      

# Line Search Method
### General Algorithm:
1. Specify some initial guess of the solution x0.
2. For k = 0, 1, ...
    
    (1) If xk is optimal, stop.
    
    (2) Determine a search direction a.
    
    (3) Determine a step length d that leads to an improved estimate of the solution: x_k+1 = x_k + ad. 
    
In its mathematical form we may write, 
####
![image](https://user-images.githubusercontent.com/88390140/131276691-f573ac2d-ed56-4795-881c-cc7e2529014b.png) 


## Rates of Convergence 
Many of the algorithms do not find a solution in a finite number of steps. 
When discussing such an algorithm, the following two questions are often asked:
1. Does it converge?
2. How fast does it converge? *Focus*
