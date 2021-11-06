## Problem 6 (technique: have you done a problem like this before? Try everything!)

Given the following substitutions:

  ABB = 7C
  
  3A7B = 24C

  A = *X*C
  
  B = *Y*C
  
Find a possible set of values for X and Y that makes the first two substitutions true, e.g. X = 5 and Y = 12. 

## Solution

In order to solve this problem, we need to somehow isolate one of the top two equations so that we only have As and Cs, but no Bs (or Bs and Cs, but no As). 

We can transform this problem into a system of linear equations. Although many of the rules of algebra (e.g. cancelling terms out)  are technically not allowed under substitution algebra, they allow us to get a "substitional-algebraically correct" answer. Let's try to "substitute away" the As in the second equation by substituting in the first equation. 

Doing so, we get B21C = 24C. Then, we can cancel out the 21 Cs on both sides, getting B = 3C. 

We can then substitute in B = 3C in the first equation, giving us A = 1C. 

Substituting these numbers back into the first two equations, we see that these values check out!

### In other words...

This problem is essentially a system of linear equations. We have A + 2B = 7, and 3A + 7B = 24. Solving this, we get A = 1 and B = 3. 
