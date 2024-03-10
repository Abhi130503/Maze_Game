1) Make use of the images saved in the folder named MazeGame_imgs (as shown in Figure 1) to design a mini game by completing the game.jpynb using medialib. Apply the knowledge of list, if statement, for and while loop for this task.
  
Figure 1
The requirement is as follows. 
The List representing the initial background of the game is   [['X','X','X','X','X','X','X','X','X','X','X','X','X','X','X','X','X','X'],
 ['X','_','F','F','_','_','M','_','_','F','F','_','F','_','_','_','_','X'],
 ['X','F','_','_','M','_','M','F','_','_','F','_','_','M','_','E','F','X'],
 ['X','_','_','F','_','_','_','_','_','F','M','_','F','_','F','_','_','X'],
 ['X','X','X','X','X','X','X','X','X','X','X','X','X','X','X','X','X','X']] 
Each character represents the name of an image. 'X ' is the location the avatar (cat) cannot pass while ’_’ is the road it can pass. The avatar will die when meeting a monster represented by ‘M’. ‘F’ represents food that can be eaten by the avatar. Draw the background of the game as shown below with the first image X.png is at (10,200). C.png represents the player's avatar and its initial position is as shown in the Figure 2. [10%] 
Figure 2
2) If the player pushes 'q', quit the game and print out “Game over!!!” [5%]
3) Control the player's avatar: [10%]
a)	if the player pushes 'a', the avatar will go backward (left). 
b)	if the player pushes 'd', the avatar will go forward (right). 
c)	if the player pushes 'w', the avatar will go upwards. 
d)	if the player pushes 's', the avatar will go downwards.
4)	If the cat stands on a position which originally has food (F.png), then the food will be eaten by the cat. When the cat leaves that position, the image of food(F.png) will be changed to the image of road(_.png). The screen should show the number of points increasing by 1 – at the start of the game there should be 0 points. [10%]

5)	Take care of illegal input. [5%]
6)	Draw the you_win.png at (100,50) when the avatar is standing on Exit (represented by E.png) [10%]

7)	Store the results of the game play in a pandas DataFrame. 
a.	Results of previous game play should be read from an excel spreadsheet into your pandas DataFrame when the game is started and should be written to the excel spreadsheet once the game is complete  [5%]
b.	Every time the game is completed a new row should added to the DataFrame before it is written to the spreadsheet [10%]
The row should include
i.	The date/time the game was played
ii.	The number of seconds taken to complete the game
iii.	The number of points (food eaten) that were scored in the game

8)	(You will need to complete at least Q7a before attempting this question.) When the game is complete, use matplotlib to visualise the data in the results DataFrame to show
a.	The distribution of game completion times in a histogram, with the most recent game time highlighted [5%]
b.	A scatterplot of game completion times against points scored [5%]
c.	A trend line for game scores, using the date/time of completion on the x axis [5%]
Include the spreadsheet storing your DataFrame with your submission: try to include some game attempts which aim to complete the game as quickly as possible, and some game attempts which aim to score as much as possible.
9)	Instead of using the initial game layout given in part 1)  choose a dataset that interests you from https://archive.ics.uci.edu/ml/index.php and use it to generate the game background.
a.	Download the dataset and include it with your submission. Include in your notebook an explanation of the source dataset and which columns you have selected. Read the dataset into a pandas DataFrame before the game is started, setting appropriate column names and types [5%]
b.	Randomly select five rows from the DataFrame containing the dataset and use two of the column values from the data set to determine the coordinates of the monsters in the background. Scale the values to make sure they are in the right range for the rows and columns of the game background. In the same way randomly select eleven rows from the dataset and use two more column values to determine the coordinates of the food [10%]
c.	Set the random seed to make sure that the same layout is achieved every time, and to ensure that it is possible to complete the game i.e. the way to the exit is not blocked by monsters [5%]
