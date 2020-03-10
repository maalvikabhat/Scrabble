SCRABBLE

SoftSys Spring 2020

Maalvika Bhat

Project 1 Update: 3/10/20

The goal of this project is to create a program in C that will produce a list of all the possible words that 
can be made from a given set of letters. It will act almost as a cheat for Scrabble (or a similar word game). 
I plan to create an easy-to-use interface where users can input upto 20 letters and a list of words 
(in alphabetic order) will be shown. A lower bound that I am confident I can acheive is the function of the 
program, and a stretch goal is to create a visually aesthetic unscrambling platform.

My learning goals are definitely to get more comfortable with C, further grapple with the idea of recursion, 
and not use an API (apart from standard functions). Since this is my first time ever working in C, I want to 
take it slow with a project that I could also do in Python. I want to get used to the way functions work in C, 
and play around a little with the permutations and combinations that are possible.

I began by finding a text file to use as a dictionary. It is essentially a list 
of words that the program can sift through to find the possible words for the letters inputted. It is downloaded
to the Github repository as dict.txt. 

I assigned frequently used variables as globals and created a count integer to keep count. Then, I found the 
longest word in the dictionary, which was 45 letters. I assigned the character word to that length. 

I set some pre-conditions so that I could easily check if the word was in the bounds of the grid. Basically, the 
code checks if the given word can be added horizontally at the given location. The pre-conditions are that the
row is a valid row location within the grid, the col is a valid column location within the grid, word is a valid 
string, num_rows is the total number of rows in the grid, num_cols is the total number of columns in the grid, and
grid is the two-dimensional array representing the grid. The post-conditions include returning true (i.e., 1) 
if the word can be added to the grid, or returning false (i.e., 0) otherwise. The grid remains unchanged. 

Tasks I am currently working on: 
a.  Checking whether word[global] can fit into the the grid at the given position. If it can, then running setWord, 
and printing grid. If not, printing an error statement. 
b.  A function which first chooses whether to place the word vertically or horizontally, and then creates an array
of structs. 
c. A function which loops through the grid, finding valid positions. For every valid position, the i,j values are 
stored in the array. Afterward, a random i,j value is chosen from the array, fed into setWord and then printGrid.

Once the functions compile and perform the way I want them to, I will know that the tasks are done. 

Trello Board: https://trello.com/b/c4Jf2kBV/scrabble
