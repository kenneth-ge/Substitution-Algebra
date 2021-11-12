## Problem 10 (technique: start small)

You're given the layout of a bunch of rooms, each of which has a wall (L), an empty space (E), and a desk (D). If each room must have at least one empty space, how many different ways are there to lay these rooms out?

S = 7(LED)

Substitution: E <-> D

## Solution
Within each room, we can have 3 different possibilities: EE, ED, and DE. 

So, our answer is 3^7. 
