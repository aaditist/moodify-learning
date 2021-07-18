# moodify-learning assignment 1
QUESTION- Virus Spread Simulation (Basic)
Create a two-dimensional matrix of dimention 100 * 150 containing 15,000 entries with value 0. Set the entry (50,75) to be 1.

8 random entries swap with another set of 8 random entries.

Visual representation

If 13 is the selected entry, 7,8,9,12,14,17,18,19 are 1st neighbours and 1,2,3,4,5,6,10,11,15,16,20,21,22,23,24,25 are 2nd neighbours.

1st neighbours of an entry containing 1 each have a 0.25 probability of getting converted to 1.

2nd neighbours of an entry containing 1 each have a 0.08 probability of getting converted to 1.

Each entry has an independent probability of getting converted to 1 depending upon its relative position to an entry containing 1.

Note that it is not mandatory for one of the neighbours to be converted into 1.

Keep repeating the process till every entry becomes 1.

Plot 1: Number of ones in the matrix vs Number of iterations

Plot 2: Change in number of ones in each iteration vs Number of iterations

Print the peak value in Plot 2. Make sure you label the axes in both the plots.


ANSWER- 

here 15000 people are considered as a matrix of 1s and 0s where 1s reperesnt the people that got infected while 0 represents the healthy people. The maximum no. of 1s added in a single iteration are returned and the plots of the total 1s after each iteration and no. of 1s added in each iteration. At first a function to swap 8 random elements in the matrix which is executed in each iteration has been created. The program iterates through the whole matrix and adds the position of elements. Then for each of those elements two functions are run, modifying the first and second neighbours, using the random.choices() function according to the given probabilities. The no. of 1s present and added after each iteration are plot using matplotlib.
