### The Goal

Your program must allow Thor to reach the light of power.

###Rules

Thor moves on a map which is 40 wide by 18 high. Note that the coordinates (X and Y) start at the top left! This means the most top left cell has the coordinates "X=0,Y=0" and the most bottom right one has the coordinates "X=39,Y=17".

**Once the program starts** you are given:

 - the variable lightX: the X position of the light of power that Thor
   must reach.
 - the variable lightY: the Y position of the light of power that Thor
   must reach.
 - the variable initialTX: the starting X position of Thor.
 - the variable initialTY: the starting Y position of Thor.

**At the end of the game turn**, you must output the direction in which you want Thor to go among:
N (North)
NE (North-East)
E (East)
SE (South-East)
S (South)
SW (South-West)
W (West)
NW (North-West)

Each movement makes Thor move by 1 cell in the chosen direction.

### Pseudo Code Algorithm

To succeed your mission, you can use this algorithm:
 
**Before the game loop**, create two variables thorX and thorY, that will hold the current position of Thor. Initialize these variables to initialTX and initialTY.
 
**For each game turn**, execute the following actions:

 - Initialize two variables of type string with two empty strings:
   directionX and directionY.

 - If thorX is greater than lightX, directionX receives the value W else if thorX is lower than lightX, directionX receives the value E.
 - If thorY is greater than lightY, directionY receives the value N else if thorY is lower than lightY, directionY receives the value S.
 - Update the variables thorX and thorY in function of the chosen direction (+1 or -1).
 - Indicate, before the end of the turn, the chosen direction as the concatenation of directionY and directionX.
