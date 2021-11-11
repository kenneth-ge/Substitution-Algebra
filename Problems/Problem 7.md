## Problem 7 (technique: what is the function? what's optimal?)

Given the following substitutions:
  ABB -> AB, AB <-> BA

And the sequence: BBBABBBBB = 3BA5B

What is the minimum value *x* you can get, where x = (the number of Bs left in your sequence at the end of all your substitutions) + (the number of substitutions it took to get there)?

## Solution
If we do nothing, we start with an answer of x = 8, since we have 8 Bs left and we've made 0 moves. 

The only action we can take to reduce this number is to reduce the number of Bs, since we can't have less than 0 moves. 

Looking at our substitutions, only the first one gets rid of a B; the second just shuffles things around. We can then remove the 5Bs to the right of the A. But, it only gets rid of 1 B in exchange for 1 move. So, our answer doesn't change. 

The second substitution would allow us to go backwards to clear the Bs on the left of the A. However, it takes one substitution to shift the A to the left, and another to clear it. So, since we're removing 1 B and adding 2 moves, it's never optimal to do this procedure. 

So, our final answer is x = 8. 
