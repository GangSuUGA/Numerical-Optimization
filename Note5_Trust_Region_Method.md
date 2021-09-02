











## Comparison:    

 Line Search Strategy | Trust Region Strategy         
----------------------|-----------------------------------------
 Choose a direction p_k     |  Construct a model function m_k (typically, quadratic) that is similar to (but simpler than) f around x_k   
 Search along p_k from x_k to x_k+1 with f(x_k+1)<f(x_k).   |  Search for x_k+1 with m_k(x_k+1)<m_k(x_k) inside a small trust region (typically a ball) around x_k.      
 Approximately solve the 1-D minimization problem: g(a)=f(x_k+a* p_k). Minimize g(a) via a subject to a>=0.   |   Approximately solve the n-D minimization problem: minimize m_k(x_k + p) via p subject to x_k + p in trust region.
  ||  If x_k+1 does not produce enough decay in f, shrink the region.  
