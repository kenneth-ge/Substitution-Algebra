## Problem 15 (technique: if the obvious solution doesn't work, think outside the box)

How do you calculate a 1 in 5 probability using only coin flips? 

## Solution

Hint 1: Try to generate a random number from 1 to 5, or from 0 to 4

Hint 2: Flipping the coin 4 times and counting heads as 1 and tails as 0 does NOT work because you’re much more likely to get 2 or 3 than you are to get 0

Hint 3: Binary numbers

Answer: 5 = 101 in base 2, which has 3 digits. So, we can flip a coin 3 times, each of which generates one of the digits. Because there’s a possibility we could end up generating a number that is greater than 5, e.g. 7, we have to “cull away” these numbers and restart the process if we see one. At the end, we can choose one number, e.g. 1, and see if we end up getting that number after every coin flip. That’ll give us one possibility out of 5. 
