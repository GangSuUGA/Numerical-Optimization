## Reference Link
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
![image](https://user-images.githubusercontent.com/88390140/131276512-5ab9af73-f79e-4dc7-a38c-d59072d8fd5b.png)
### Example
![image](https://user-images.githubusercontent.com/88390140/131276552-f931019e-8b4b-4d8a-9024-7576b7728aea.png)

## Secant Method
Just like Newton’s method the secant’s method to find the minimum is given by:
### Example 
