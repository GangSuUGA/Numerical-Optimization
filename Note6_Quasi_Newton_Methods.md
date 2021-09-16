# References Links:
 - 

______________________________________

 - Quasi-Newton Methods, like steepest descent, require only the gradient of the objective function to be supplied at each iterate. 
 - By measuring the changes in gradients, W.C. Davidon construct a model of the objective function (**an approximation B_k to the Hessian Matrix**) that is good enough to produce superlinear convergence.        
 - Moreover, since second derivatives are not required, quasi-Newton methods are sometimes more efficient than Newton's method. 
 - Today, optimization software libraries contain a veriety of quasi-Newton algorithm for solving unconstrained, constrained and large-scale optimization problems. 

## New Quadratic model:      
![image](https://user-images.githubusercontent.com/88390140/133532045-5ef577db-3b44-48b6-bf91-7408cdc52c78.png)

![image](https://user-images.githubusercontent.com/88390140/133532184-bd4323f4-a38a-44cb-947e-ef398353d0aa.png) or Infer from Second Derivitive Equation. 

![image](https://user-images.githubusercontent.com/88390140/133532250-9c3ec508-37cc-4102-95b8-3383f773d1eb.png)

## Key Point: 
![image](https://user-images.githubusercontent.com/88390140/133532650-91dd26a1-43bd-421d-92ec-526d72b499d5.png)

## Three Popular Methods to solve B_k: 
- DFP
- **BFGS**
- SR1


