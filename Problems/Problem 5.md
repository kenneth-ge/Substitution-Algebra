## Problem 4 (technique: what must happen? what cannot happen?)

Many words in the English language often take the form of a prefix, a base word, and a suffix. For example, "redistricting" can be broken up into "re-," "district," and "-ing." In substitution algebra, you can express a word of this form as ABC, where A represents the prefix, B represents the base word, and C represents the suffix. 

### Part A: 
Given the base word "K," and prefixes A through J and suffixes L through Z, how many possibilities are there?

### Part B: 
Choose a base word of your own, then come up with a list of prefixes and suffixes (these don't have to make sense! For example, "preselfieify" and "literaturally" both work!). Then, list out a set of transformations to get you there, starting with the structure we used above of ABC. 

## Solution

Answer to part A: A - J gives us 10 prefixes, and L - Z gives us 15 suffixes. So, we have a total of 10 * 15 + 10 + 15 + 1 combinations. That's because we have four total cases here: 
1. Leave the base word as is (1 possibility)
2. Use just a suffix (15 possibilities)
3. Use just a prefix (10 possibilities)
4. Use a prefix and a suffix (15 * 10 = 150 possibilities)


Answer to part B: An example is the following:

S = {

A = ""

B = "literature" (drop the "e" at the end if appropriate)

C = ""

}



T = {

  A <-> "pre" <-> "re" <-> "post"
  
  C <-> "ally" <-> "ify"
  
}
