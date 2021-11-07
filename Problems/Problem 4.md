## Problem 4 (technique: what must happen? what cannot happen?)

S = ABLCDLCDLCDLE

T = {
  BL <-> DL
}

How many possibilities for S are there such that all of the letters (excluding all the Ls) are one away from each other (contiguous, connected) in the alphabet? E.g. B is one away from A and C

## Solution

Answer: 4; the first letter has to be a B, and the second and third letters can be a B or a D. The fourth letter has to be a D, because otherwise B is three letters away from E, so it wouldn't work. 
