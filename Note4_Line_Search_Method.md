## Resources Link
 - [**Line Search Methods 1**](https://optimization.mccormick.northwestern.edu/index.php/Line_search_methods)  
 - [**Line search Methods 2**](https://sites.math.washington.edu/~burke/crs/408/notes/nlp/line.pdf)
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

# Direction 

For most algorithm, p_k = - B_k^-1 * ![image](https://user-images.githubusercontent.com/88390140/132270272-0ad70cb8-0f0d-423d-9bd3-f2d32ae8bdb9.png), where B_k is symmetric and non-singular. 

 - For SD (Steepest Descent): B_k = I    
 - For original Newton Method: B_k = ![image](https://user-images.githubusercontent.com/88390140/132270256-caa4aad4-cc40-4878-83ff-295a21191c76.png) 
 - For Quasi Newton Method: B_k ~= ![image](https://user-images.githubusercontent.com/88390140/132270256-caa4aad4-cc40-4878-83ff-295a21191c76.png)  

**If B_k is positive definite, then P_k is a descent directionL**    

## Descent Direction: 
Note p_k is a **descent direction**. And the properity is:       
![image](https://user-images.githubusercontent.com/88390140/131768167-7091d28c-3bea-454e-9e5f-fe4a9f1caec8.png), which will guarantees that f can be reduced along p_k.    
       
**Proof:**      
(1) The inner(dot) product less than 0 in two situation:
 - The angle between two vector is opposed.      

(2) From the perspective of taylor's eries in matrix form:        
 - f(x_k+1) = f(x_k + a_k * p_k) ~= f(x_k) + a_k * ![image](https://user-images.githubusercontent.com/88390140/131769443-ad54a67f-37d9-4c88-9934-87facce87795.png) + ......            
 - Given a_k >= 0, so if we want f(x_k+1) < f(x_k), ![image](https://user-images.githubusercontent.com/88390140/131768167-7091d28c-3bea-454e-9e5f-fe4a9f1caec8.png) must be satisfy. This completes the proof.  

## Newton's Method: 
![image](https://user-images.githubusercontent.com/88390140/132270256-caa4aad4-cc40-4878-83ff-295a21191c76.png) * p_k = - ![image](https://user-images.githubusercontent.com/88390140/132270272-0ad70cb8-0f0d-423d-9bd3-f2d32ae8bdb9.png)

Finding the inverse of the Hessian in high dimensions to compute the Newton direction ![image](https://user-images.githubusercontent.com/88390140/132270256-caa4aad4-cc40-4878-83ff-295a21191c76.png) * p_k = - ![image](https://user-images.githubusercontent.com/88390140/132270272-0ad70cb8-0f0d-423d-9bd3-f2d32ae8bdb9.png)  can be an expensive operation. In such cases, instead of directly inverting the Hessian, it is better to calculate the vector ![image](https://user-images.githubusercontent.com/88390140/132270272-0ad70cb8-0f0d-423d-9bd3-f2d32ae8bdb9.png) as the solution to the system of linear equations

_________________________________________

# Step Length: 

To cope with how to choose the step length given the search direction p_k, desirable properties include guaranteed global convergence, and rapid rate of convergence (Trade-off: time & accuracy):     
want to choose a_k to give a substantial reduction in f, but not to spend much time on it.    
 - **Exact line search** (global and local min): Too expensive
 - **Inexact line search**: A typical line search algorithm will try a sequence of a's and step when certain conditions hold. (Wolfe or Strong Wolfe Conditions) 




