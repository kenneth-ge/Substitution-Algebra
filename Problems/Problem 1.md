## Problem 1 (technique: induction, proofs, invariants, conservation)

Given the starting sequence S = AALB, and the transformation AL -> AALB, prove that after x substitutions, you get the sequence (x+2)AL(x+1)B

## Solution

Let's think first about the problem-solving technique of conservation in our substitution up above. If we take a look at AL -> AALB, notice that there is 1 A on the left side and 2 As on the right. That means we gain a single A every time we apply the substitution. The same is true with B. So, after x substitutions, we have an extra x As and x Bs, so we have (x + 2) As and (x + 1) Bs. 

Now, let's prove that the structure of the final product is a series of As, then an L, then a series of Bs. Let's take a look at the L, our invariant. In the substitution, the only time we ever see As on either side is to the left of the L, and the only time we ever see Bs is to the right of the L. So, applying the substitution multiple times lengthens the sequence, but doesn't change the structure. 

QED
