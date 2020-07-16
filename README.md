# Data-Structure-and-Algorithm

Which one of them is the better one ?    
> Factors :  
> 1. Different programming Languages -> Programmer writes bad code in C run faster in fast machine  
> 2. Running on different machines  

Therefore , theoretical analysis and mathematical tools helps in determining better code , so that you do not depend upon programming language and machine. The analysis which helps in determining this is called Asymptotic Analysis.

## Big O Notation (Upper Bound)

We say f(n) = O(g(n)) iff there exists constants c and n∘  such that f(n) <= cg(n) for all n>=n∘   

![Screenshot 2020-07-16 at 11 33 21 PM](https://user-images.githubusercontent.com/68182511/87706536-4f376c00-c7bd-11ea-9e0d-1c04ff6099ea.png)

1. f(n) = 3n² + 4n + 100  
   Ignore the lower order term and all constant   

   f(n) = O(n²)  

2. f(n) = 3n + 4logn + 140     
   f(n) = O(n)  
     
```
int linearsearch(int x,int arr[],int n)
{
    for(int i=0;i<n;i++)
    if(arr[i]==x)
    return i;
 return -1;   
}
```  
The above code is O(n). As O(n) is __upper bound__ it covers everything i.e. best case (c), average case. That's why it is the most used notation.  

{3n², 4n², 3n²/2, log(n), 2log(n)} ∈ O(n²) -> This indicates that lower order comes under O(n²) as well.  

## Omega Notation (Lower Bound)  

We say f(n) = Ω(g(n)) iff there exist positive constants c and n∘ such that 0 <= cg(n) <= f(n) for all n>=n∘  
 
![Screenshot 2020-07-17 at 12 37 20 AM](https://user-images.githubusercontent.com/68182511/87712099-d4bf1a00-c7c5-11ea-8674-08fde32c31ed.png)

{n, n/2, 3n², 4n²/5, n³,...} ∈ O(n) -> This indicates that higher order comes under O(n) as well.  

f(n) = Ω(g(n))
g(n) = O(f(n))  




