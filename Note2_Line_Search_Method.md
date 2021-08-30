https://optimization.mccormick.northwestern.edu/index.php/Line_search_methods
http://www.cas.mcmaster.ca/~cs4te3/notes/LineSearchMethods.pdf

## Bisection Method
In bisection method we reduce begin with an interval so that 0 ∈ [a, b] and divide the interval in two
halves,i.e. [a, (a+b)/2] and [(a+b)/2 , b]. A next search interval is chosen by comparing and finding which one
has zero. This is done by evaluating the sign. The algorithm for this is given as follows: Choose a, b
so that f(a)f(b) < 0
### Example
![image](https://user-images.githubusercontent.com/88390140/131276423-2a2afcc8-0e2b-4c51-a905-769d985c5b51.png)
