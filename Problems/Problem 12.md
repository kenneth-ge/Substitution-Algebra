## Problem 12 (technique: visualize, what are the only valid possibilities?)

You're given a sequence S = 10(AB), and the substitutions ABA = CBC, ADA = CDC, BAB = DAD, BCB = DCD, and AB = EE. 

After using a series of the substitutions above, what is the minimum number of letters in the sequence (these can be any letter, they don't have to be in order) that you need to check in order to determine whether there are any Es?

## Solution

For a brief explanation of what these substitutions do, please consult question 11. Ready? Awesome. 

So, basically, given some kind of an end result, we want to know how many letters in the sequence we have to check to determine whether or not there is at least one E. 

The first naive idea is that, since adding Es to the sequence basically adds a vertical line, we can just check all the top rows and see if there are any Es there. Since every E in the bottom row corresponds with an E in the top row, we should be good!

However, remember our catch from problem 11 -- if we take a sequence of Es, and only replace the middle portion with EE = AB, we might be left with a situation where we have an E on the top, but an A on the bottom. 

But, it feels like we were getting somewhere with our "check half the sequence" idea. Let's prove that you only need to check half the sequence. 

Well, since every E comes in a pair, clearly, if we have an E somewhere, it's going to correspond to an E somewhere else. Regardless of whether it's in the bottom half, we should have an E somewhere else in the sequence. Intuitively, we can't check any less than half, since we could miss one of these pairs. 

Let's take a closer look at the cases that break our initial, naive idea. In these cases, the board looks something like this:

EBBB

AAAE

In this case, we have an E on the top, and it does still in fact correspond with an E on the bottom -- just not directly below. Intuitively, this makes sense -- if we're making Es by putting two of them next to each other (aka one on each row), and we can only add/remove Es in pairs, there's always going to be one E on the top row, and another on the bottom. 

So, our naive idea to check just the top row does, indeed, work. We just had to go through a few steps to prove it. 
