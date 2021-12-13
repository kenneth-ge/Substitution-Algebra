## Problem 14 (technique: invariants, conservation)

Given S = AAAAA, and the substitutions A = B = C, come up with a Roman numeral-style system that maximizes your total range. A Roman-numeral-style system means each letter has a whole number value >= 0, e.g. A = 1, B = 6, C = 10, and you can obtain the total value of a set of numerals by adding up the individual values of each one. A Roman numeral system has a "range" of x if it can be used to represent all integer numbers from 1 up to and including x. Also, note that you must have exactly 5 numerals. 

Prove that your answer is optimal. 

## Solution

To start off, let's organize our thinking by making our lowest value numeral A, our second-lowest B, and our greatest C. 

Our first important observation is that there are exactly five numerals in our number. This means our lowest possible answer is 5 * A. An initial thought might be to make A = 1. However, our minimum value then becomes 5 * A = 5. So, because of this, A has to be equal to zero. 

Now that we can represent zero, we then need to be able to represent 1, 2, 3... If we choose a large number for B, e.g. B = 50, then clearly, there's no way to flil in the gaps between 0 and 50 because we don't have anything lower. Even if we chose B = 2, we still wouldn't able to obtain a value of 1, since the second-lowest possible value is then AAAAB = 2. So, B has to be equal to 1. 

Choosing a value for C is the trickiest part. To get a better idea for what kind of value we should pick, let's try setting C arbitrarily equal to 2, and then getting a feel for what counting looks like:

| Numerals    | Number      |
| ----------- | ----------- |
| AAAAA | 0 |
| AAAAB | 1 |
| AAABB | 2 |
| AAAAC | 2 |
| AAABC | 3 |
| AABBC | 4 |
| AAACC | 4 |
| ... | ... |
| ABCCC | 7 |
| BBCCC | 8 |
| ACCCC | 8 |
| BCCCC | 9 |
| CCCCC | 10 |

Notice that the C basically takes the place of 2 Bs, since C has the same value of 2 Bs. So, by replacing BB = C, we can add room for one extra letter, which is a B. Since 2 clearly works (and gives us a range of 10), let's try C = 5. 

| Numerals    | Number      |
| ----------- | ----------- |
| AAAAA | 0 |
| AAAAB | 1 |
| AAABB | 2 |
| AABBB | 3 |
| ABBBB | 4 |
| AAAAC | 5 |
| ... | ... |
| AABCC | 11 |
| ABBCC | 12 |
| BBBCC | 13 |
| ????? | 14 |
| AACCC | 15 |

Whoops! We ran out of space! In order to get from 13 to 14, we need to incorporate one extra B. There's no other way to do it because we're already packing all the Cs that we can into the sequence. However, we can't pack an extra B, because we only have 5 letters total. So, our total range is 13. 

But can we do better? Let's think about this. In essence, our maximum value comes about when we run out of space. In this case, we needed to have at least 4 "empty" spaces, since C has a value of 5. However, we only had 3 = (C - 2). 

Generalizing this conclusion, our maximum range is 1 * (C - 2) + C * (7 - C). This is because we stop counting when we have C - 2 total Bs, and the rest of the \{5 - (C - 2)\] = (7 - C) letters are all Cs. 

So, let's maximize our equation: C - 2 + 7C - C^2 = -C^2 + 8C - 2. Since we can't use any C values 7 or above (prove this to yourself), we just need to plug in C values that range from 2 to 6. Alternatively, we could use calculus to maximize this equation. 

Eventually, we get our answer, which is C = 4, giving us a total range of -16 + 32 - 2 = 14. 
