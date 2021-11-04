## Problem 3 (technique: notice the pattern)

You’re given the sequence of letters AAAAAAAAAABBAAAAAAAAAA. At any point in time, you can swap BBA for ABB or vice versa. If you have to do exactly 4 of these swaps, how many distinct sequences of letters can you end up with?

An example of how you might use the swaps: if you had the sequence AABBAA, you could apply BBA -> ABB once to get AAABBA, and you could apply it again to get AAAABB.

## Solution

Answer: 5, since you can shift it an even number of times to the left or right. So, you can shift it right two spaces, left two spaces, or keep it in the same space. 
