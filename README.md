# 2048
					2048 GAME

IMPLEMENTATION OF LOGIC PART
1.	Initialized a 4*4 matrix with all elements as 0
2.	Generating a random 2 at a random empty position using the random library and randint functionality ( depends upon whether a change happened or not here, change referrers to compression or merging )
3.	Getting the current state of a game at every move we need to check the current state of a game, it will return three things	
a.	Won  2048 in one of the cells 
b.	Game over 
c.	Game still not over  empty cells or consecutive elements are same as they can combine and create an empty position
4.	Compressing  create and return a new matrix, iterate through the old matrix, and if an element is non zero replace it in the new matrix of the same row at a position p, this will move all the non-zero numbers at the left side
5.	Merging we will check for each row if consecutive elements are the same then double the element at that position and empty the other
6.	Reversing return a new_matrix
7.	Transposing return a new_matrix
8.	Implementing all the moves ( we can generalize all the moves once we know how to make a left move)
a.	LEFT 
i.	Compress
ii.	Merge
iii.	Compress
b.	RIGHT
i.	Reverse
ii.	Compress
iii.	Merge
iv.	Compress
v.	Reverse
c.	UP
i.	Transpose
ii.	Compress
iii.	Merge
iv.	Compress
v.	Transpose
d.	DOWN
i.	Transpose
ii.	Reverse
iii.	Compress
iv.	Merge
v.	Compress
vi.	Reverse
vii.	Transpose
9.	Change or no change After any move a new 2 will come or not will depend on weather some change happened or not (change means Compression or merging) 


CONSTANTS
Generalized code that contains all the parameters that we will be using in our actual code for the UI part
					    UI PART
Using Tkinter Library and importing some libraries Label, Frame, Center
Tkinter allows us to create a UI
The frame allows us to create a box kind of thing in which we can place all our widgets
self.grid() Tkinter has a grid manager which allows us to create all our widgets in the form of grids that is I have initialized our frame as a grid
Then I have used the master functionality to bind it means whenever a key is pressed within this frame it will reflect into the UI part 




