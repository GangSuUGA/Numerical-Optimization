## Resources Link
#### Line Search Method: https://optimization.mccormick.northwestern.edu/index.php/Line_search_methods     
#### Convergence of Algorithms: https://caam37830.github.io/book/01_analysis/convergence.html#:~:text=Many%20numerical%20algorithms%20converge%20to%20a%20solution%2C%20meaning,k%20%E2%86%92%20%E2%88%9E%20%CF%B5%20k%20%3D%200%20%24      
#### Algorithms and their convergence: http://macs.citadel.edu/chenm/343.dir/11.dir/lect1_3.pdf      
___________________________________________________________________________________________________________________________________________________________________________________

**Sometime, problem is so complex that made function/formula cannot be expressed generally and explicitly. Previous method, which find the first-derivative equal to 0, can not work.**   

Here will introduce two Fundemental Strategies, **Line Search Method** and **Trust Region Method**.    

## Algorithm: 
1. Specify some initial guess of the solution x_0.     
2. For k = 0, 1, ...     
    (1) If x_k is optimal, stop.     
    (2) Determine x_k+1, a search direction p_k       
    (3) Determine a step length a_k, then ![image](https://user-images.githubusercontent.com/88390140/131768255-27daccad-65f5-40dc-83fa-bf92ac37d32d.png) 
       
       
#### Each iteration of a line search method computes a search direction p_k and then decides how far to move along that direction.    
      
 ## Mathematical form:        
 -  Line Search Method:      
![image](https://user-images.githubusercontent.com/88390140/131764100-aa19cf9f-3a73-48bd-a747-3e5b06418faa.png)      
     
Note p_k is a **descent direction**. And the properity is:       
![image](https://user-images.githubusercontent.com/88390140/131768167-7091d28c-3bea-454e-9e5f-fe4a9f1caec8.png), which will guarantees that f can be reduced along p_k.    
       
**Proof:**      
(1) The inner(dot) product less than 0 in two situation:
 - (a) gradient > 0, we should choose the opposed direction.   
 - (b) gradient < 0, we should choose the same direction.       

(2) From the perspective of taylor's eries in matrix form:        
 - f(x_k+1) = f(x_k + a_k * p_k) ~= f(x_k) + a_k * ![image](https://user-images.githubusercontent.com/88390140/131769443-ad54a67f-37d9-4c88-9934-87facce87795.png) + ......            
 - Given a_k >= 0, so if we want f(x_k+1) < f(x_k), ![image](https://user-images.githubusercontent.com/88390140/131768167-7091d28c-3bea-454e-9e5f-fe4a9f1caec8.png) must be satisfy. This completes the proof.  


