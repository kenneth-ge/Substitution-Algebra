## Problem 13 (technique: experiment)

Given just the following substitution:
  
  A = B = C
  
Part A: Come up with a sytsem of counting that allows you to count to at least 14 with just the following sequence:

  AAAAA
  
Part B: What if we wanted to count to 50? 100? Does your answer change?

For clarification, counting to 15 means you can start at 1, then use some kind of a rule or formula (e.g. A = 1) such that you have a sequence that corresponds to each number between 1 and 15. 

## Solution

For 15, we could pretty easily use a Roman numeral-type system. For example, we can create a system where A represents 0, B represents 1, and C represents 4. That way, we have:

| Number      | Numerals    |
| ----------- | ----------- |
| 1           | AAAAB       |
| 2           | AAABB       |
| 3           | AABBB       |
| 4           | AAAAC       |
| 5           | AAABC       |
| 6           | AABBC       |
| 7           | ABBBC       |
| 8           | AAACC       |
| 9           | AABCC       |
| 10          | ABBCC       |
| 11          | BBBCC       |
| 12          | AACCC       |
| 13          | ABCCC       |
| 14          | BBCCC       |

To find others, feel free to experiment!

For larger numbers, we can actually turn these letters into digits, where A = 0, B = 1, and C = 2. That way, AAAAA = 00000, AAAAB = 00001, etc. 

Investigating this further, we can see that we've actually created a base 3 number system. So, we can count any number between 0 and 22222_3, which is equal to 242. 

If we wanted to go one further, we could also shift all of these numbers up. In other words, we can add 1 to each of these number so that AAAAA = 1, AAAAB = 2, etc. This gives us a maximum value of 243. 

Unfortunately, we can't go any further, since there are only 3^5 = 243 total permutations of this sequence. But hey, that's still a pretty large number considering we started with just AAAAA, and counted with our ABCs. 
