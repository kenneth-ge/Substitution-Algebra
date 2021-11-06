## Problem 4 (technique: have you done a problem like this before? Try everything!)
Given the following substitutions:
  ABB = 7C
  
  3A7B = 24C
  
  AB = BA
  
  AC = CA
  
  BC = CB
  

Find A and B in terms of C. I.e. you should get an answer in the form of A = 10C, B = 40C. 

## Solution
We can solve this problem in two ways. We can either work within substitution algebra, or we can transform this into a system of linear equations. Let's try both. 

### Working Within Substitution Algebra
In order to solve this problem, we need to somehow isolate one of the top two equations so that we only have As and Cs, but no Bs (or Bs and Cs, but no As). 

Notice that the last three substitutions basically allow us to swap adjacent letters. Let's try to "substitute away" the As in the second equation by substituting in the first equation. 

Doing so, we get B21C = 24C. Then, we can cancel out the 21 Cs on both sides, getting B = 3C. 

We can then substitute in B = 3C in the first equation, giving us A = 1C. 

## Transforming The Problem
This problem is essentially a system of linear equations. We have A + 2B = 7, and 3A + 7B = 24. Solving this, we get A = 1 and B = 3. 
