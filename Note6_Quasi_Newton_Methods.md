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

## DFP: 

![image](https://user-images.githubusercontent.com/88390140/133534014-0c198c04-045a-43cb-b411-c49f91f47bd9.png)
![image](https://user-images.githubusercontent.com/88390140/133534036-0ab1a3cc-dbf0-490d-b2f7-36ad39b185c3.png)      
![image](https://user-images.githubusercontent.com/88390140/133534113-536e4327-71ad-403e-9d9c-f1ad3034ddd6.png)

Instead of recomputing the approximate Hessians from scratch at every iteration, we apply a simple modification that combines the most recently observed information about the objective function with the existing knowledge embedded in our current Hessian approximation.       

## **BFGS**: 
Remark: With an adequate line search (e.g., wolfe conditions), BFGS has effective self-correcting properties (but DFP is not so effective).    
More effiective of all quasi-Newton updating formula, BFGS, can be derived by making a simple change in the DFP formula.        
**Instead of imposing conditions on the Hessian approximations B_k, we impose similar conditions on the inverses H_k (Note: Not Hessian).**   
![image](https://user-images.githubusercontent.com/88390140/133534724-b915a1bb-3c0b-4afb-a8fb-2f507bae2240.png)
![image](https://user-images.githubusercontent.com/88390140/133534737-3c8346bc-9f58-4d31-b9d0-5c59a972c277.png)


![image](https://user-images.githubusercontent.com/88390140/133534999-af6a091c-5d6d-43bd-8a4b-1f2aefb1dd50.png)
![image](https://user-images.githubusercontent.com/88390140/133535015-31fd09b4-599d-4fcc-8aef-290014716cd2.png)
![image](https://user-images.githubusercontent.com/88390140/133535296-f53edda9-9764-4009-b413-ff1d36a0c848.png)

## SR1: 




