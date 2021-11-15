## Problem 11 (technique: list your assumptions, and visualize)

You're given a sequence S = 10(AB), and the substitutions ABA = CBC, ADA = CDC, BAB = DAD, BCB = DCD, and AB = EE. 

Your goal is to use these substitutions to get rid of all the As and Bs on the board. Then, once those are all gone, you are to count the number of Cs, Ds, and Es that are left over. Maximize the product of these three counts. 

## Solution
We can visualize this as a set of two rows, the top row being 10 As and the bottom row being 10 Bs. 

ABABABABABABABABABAB = 

AAAAAAAAAA

BBBBBBBBBB



Then, these substitutions basically become:

* ABA = CBC replaces two consecutive As with Cs
  
* BAB = DAD replaces two consecutive Bs with Ds
  
* AB = EE replaces two letters that are together vertically with Es. 
  
* ADA = CDC and BCB = DCD just work as helper substitutions in conjunction with the top 2. 
  
Essentially, our goal is to place as many 2x1 pieces on top of a board as possible such we have as diverse of a selection of different orientations of these pieces as possible. 

You might be thinking: Okay, the first four substitutions make sense because they're independent, but wouldn't the fourth substitution mess things up?

And right you are for asking that question to yourself! It does seem like this could mess things up. In fact, we could end up with a situation like this (I've simplified the board down to just 5 As and 5 Bs):

ABEEEEEEAB = ABEABABEAB = 

AEBBA

BAAEB

Oh no! We've swapped our As and Bs onto different rows! Luckily, this doesn't pose an issue. Since we're only concerned about maximizing the product of these three numbers, it doesn't actually matter what configuration we choose exactly, so we could have Cd on the bottom and Ds on the top, and the math would still work out all the same (although, we will still keep exploring this concept in the next problem!). 

So, since we have 10 of each number, which is 20 characters total, to maximize the product, the best way is just to produce an even split. In this case, we want 7 of one number, 7 of another, and 6 of the last one. However, since all of our substitutions change two letters at a time, the best we can do it 8, 6, and 6. So, our answer is 8 * 6 * 6 = 288. 
