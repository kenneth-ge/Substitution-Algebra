## Problem 4 (technique: what must happen? what cannot happen?)

S = ABLCDLCDLE

T = {
  BL <-> DL
}

How many combinations are there such that all of the letters (excluding L) are one away from each other (contiguous, connected) in the alphabet? E.g. B is one away from A and C

## Solution

Answer: 2; the first letter has to be a B, and the second letter can be a B or a D. The third letter has to be a D, because otherwise B is three letters away from E, so it wouldn't work. 
