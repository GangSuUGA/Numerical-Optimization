## Resources Link   
#### Root-finding: http://www.cas.mcmaster.ca/~cs4te3/notes/LineSearchMethods.pdf 
___________________________________________________________________________________________________________________________________________________________________________________


# Zero/Root Finding

## Background     
Assuming already explictly known what f is and that f is smooth and continuous, all we need to do is to find its optimum where its first-derivative is zero, i.e. ∇f(x) = 0. In other words, we are trying to find zero of the derivative function (i.e. the point where the dereviative function intersects the x−axis).     
We will visit some known **zero-finding (or root-finding)** techniques when the root equation is not easily to solve. 

## General Optimization Algorithm:
1. Specify some initial guess of the solution x0.    
2. For k = 0, 1, ...      
    (1) If xk is optimal, stop.     
    (2) Determine xk+1, a new estimate of the solution.     


## Bisection Method
In bisection method we reduce begin with an interval so that 0 ∈ [a, b] and divide the interval in two
halves,i.e. [a, (a+b)/2] and [(a+b)/2 , b].  
A next search interval is chosen by comparing and finding which one
has zero. This is done by evaluating the sign. The algorithm for this is given as follows: Choose a, b
so that f(a)f(b) < 0
### Example
![image](https://user-images.githubusercontent.com/88390140/131277886-6d08f12a-612e-41fe-8db4-fd820ed15db5.png)

## Newton's Method
Newton’s method to find the minimum uses the first derivative of the approximation an equalling it to zero. 
![image](https://user-images.githubusercontent.com/88390140/131277162-69dc4d0e-2b96-420c-9f95-1224fa2cfe4d.png)
### Example
For a smooth, continuous function when proper starting point is chosen, Newton’s method can be real fast. ![image](https://user-images.githubusercontent.com/88390140/131277481-a7004d75-8efc-4cb2-b205-bf7396555407.png)
![image](https://user-images.githubusercontent.com/88390140/131277533-c1c8835f-1b6a-4719-9d94-4740b7e7ecde.png)

## Secant Method
Just like Newton’s method the secant’s method to find the minimum is given by:
#### ![image](https://user-images.githubusercontent.com/88390140/131276891-f0444bcc-17c7-4727-811c-b24b9a1ce4e8.png)
### Example 
![image](https://user-images.githubusercontent.com/88390140/131276913-cadf5769-89ac-4013-9749-4ce71c826e39.png)
![image](https://user-images.githubusercontent.com/88390140/131278001-3d9c2fde-79f8-4f25-bbb3-3b1b6565e4b9.png)

## Golden Section Method 
### Example 
![image](https://user-images.githubusercontent.com/88390140/131276982-5b1a6626-a759-498a-9488-5b469510fad2.png)
### Another Example 
![image](https://user-images.githubusercontent.com/88390140/131277023-77176060-cfdd-4fff-ad03-4633711bc41c.png)
![image](https://user-images.githubusercontent.com/88390140/131277036-e3b8df5d-d01a-48b1-81b8-f83a816fa69c.png)
