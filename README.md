# River-Crossing-The-Generalized-Missionaries-and-Cannibals-Problem

If you like logic puzzles or are a student of computer science (why, hello!), you've probably heard of river crossing problems such as: The Jealous Husbands; Fox, Goose and Bag of Beans; Wolf, Goat and a Cabbage; or the Missionaries and Cannibals problem.

We'll be looking at the Missionaries and Cannabals problem, which is typically stated something like this:

Three missionaries and three cannibals must cross a river using a boat, which can carry at most two people. There is a constraint that, for both banks, if there are missionaries present on the bank, they cannot be outnumbered by cannibals. (If they were, the cannibals would eat the missionaries.) 

How can the boat be used to safely carry all the missionaries and cannibals across the river?
There are only two valid moves in the game: Boat crossing with X missionaries and Y cannibals and boat returning with X missionaries and Y cannibals.

A solution for that particular problem (in case you haven't worked it out in your head)...

#The Missionaries and Cannibals Problem
0:3M 3C<> ~~~~~~~~~~~~ __0M 0C

1M 1C ->

1:2M 2C__ ~~~~~~~~~~~~ <>1M 1C

<- 1M 0C

2:3M 2C<> ~~~~~~~~~~~~ __0M 1C

0M 2C ->

3:3M 0C__ ~~~~~~~~~~~~ <>0M 3C

<- 0M 1C

4:3M 1C<> ~~~~~~~~~~~~ __0M 2C

2M 0C ->

5:1M 1C__ ~~~~~~~~~~~~ <>2M 2C

<- 1M 1C

6:2M 2C<> ~~~~~~~~~~~~ __1M 1C

2M 0C ->

7:0M 2C__ ~~~~~~~~~~~~ <>3M 1C

<- 0M 1C

8:0M 3C<> ~~~~~~~~~~~~ __3M 0C

0M 2C ->

9:0M 1C__ ~~~~~~~~~~~~ <>3M 2C

<- 0M 1C

10:0M 2C<> ~~~~~~~~~~~~ __3M 1C

0M 2C ->

11:0M 0C__ ~~~~~~~~~~~~ <>3M 3C

Safely crossed the river with 11 crossings.

#The Generalized Missionaries and Cannibals Problem
Given M missionaries, C cannibals, and P people per boat capacity, give the sequence of actions for crossing the river safely.

Some notes:

For scenarios of P >=3, if there are missionaries present on the boat, they cannot be outnumbered by cannibals. (Same rule as the banks.)
After a boat crossing, all passengers must disembark onto the shore, therefore a boat cannot be used as a safe place.
The boat cannot cross the river by itself. You need at least one rower.
Not EVERY combination of M, C, and P is solvable.
Solutions are not necessarily unique, but your solution must be a minimum crossings solution.

#Test Cases:

3 3 3 Solution 5 moves

20 20 4 Solution 37 moves

4 4 2 No solution 

5 5 3 Solution 11 moves

2 3 2 No Solution


