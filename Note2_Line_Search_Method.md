## Resources Link
https://optimization.mccormick.northwestern.edu/index.php/Line_search_methods
http://www.cas.mcmaster.ca/~cs4te3/notes/LineSearchMethods.pdf

# Line Search Method
In its mathematical form we may write, 
####
![image](https://user-images.githubusercontent.com/88390140/131276691-f573ac2d-ed56-4795-881c-cc7e2529014b.png)
####
Assuming that f is smooth and continuous, we find its optimum where its first-derivative is zero, i.e. ∇f(x +
αd) = 0. All we are doing is trying to find zero of a function (i.e. the point where the curves intersects
the x−axis). We will visit some known and some newer zero-finding (or root-finding) techniques.


## Bisection Method
In bisection method we reduce begin with an interval so that 0 ∈ [a, b] and divide the interval in two
halves,i.e. [a, (a+b)/2] and [(a+b)/2 , b]. A next search interval is chosen by comparing and finding which one
has zero. This is done by evaluating the sign. The algorithm for this is given as follows: Choose a, b
so that f(a)f(b) < 0
### Example
![image](https://user-images.githubusercontent.com/88390140/131276423-2a2afcc8-0e2b-4c51-a905-769d985c5b51.png)

## Newton's Method
Newton’s method to find the minimum uses the first derivative of the approximation an equalling it to zero. 
![image](https://user-images.githubusercontent.com/88390140/131277162-69dc4d0e-2b96-420c-9f95-1224fa2cfe4d.png)
### Example
![image](https://user-images.githubusercontent.com/88390140/131277235-df66aadf-ef1e-4f76-8da9-14fb3c4f75f9.png)
![image](https://user-images.githubusercontent.com/88390140/131277293-16b7656b-77cb-41e4-91e8-890b91b87490.png)
![image](https://user-images.githubusercontent.com/88390140/131277330-8ab75e4e-43df-4734-85be-2b440c797015.png)
![image](https://user-images.githubusercontent.com/88390140/131277339-f0b32ee9-a732-458e-beb8-0fa9f373376e.png)

## Secant Method
Just like Newton’s method the secant’s method to find the minimum is given by:
#### ![image](https://user-images.githubusercontent.com/88390140/131276891-f0444bcc-17c7-4727-811c-b24b9a1ce4e8.png)
### Example 
![image](https://user-images.githubusercontent.com/88390140/131276913-cadf5769-89ac-4013-9749-4ce71c826e39.png)
![image](https://user-images.githubusercontent.com/88390140/131276923-4e80b04a-d0b4-459b-8089-6aae47925501.png)

## Golden Section Method 
### Example 
![image](https://user-images.githubusercontent.com/88390140/131276982-5b1a6626-a759-498a-9488-5b469510fad2.png)
### Another Example 
![image](https://user-images.githubusercontent.com/88390140/131277023-77176060-cfdd-4fff-ad03-4633711bc41c.png)
![image](https://user-images.githubusercontent.com/88390140/131277036-e3b8df5d-d01a-48b1-81b8-f83a816fa69c.png)
