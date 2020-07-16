# Data-Structure-and-Algorithm

Which one of them is the better one ?    
> Factors :  
> 1. Different programming Languages -> Programmer writes bad code in C run faster in fast machine  
> 2. Running on different machines  

Therefore , theoretical analysis and mathematical tools helps in determining better code , so that you do not depend upon programming language and machine. The analysis which helps in determining this is called Asymptotic Analysis.

## Big O Notation

We say f(n) = O(g(n)) iff there exists constants c and no such that f(n) <= cg(n) for all n>=no  

![Screenshot 2020-07-16 at 11 33 21 PM](https://user-images.githubusercontent.com/68182511/87706536-4f376c00-c7bd-11ea-9e0d-1c04ff6099ea.png)

1. f(n) = 3n² + 4n + 100  
   Ignore the lower order term and all constant   

   f(n) = O(n²)  

2. f(n) = 3n + 4logn + 140  
    
   f(n) = O(n)  
   