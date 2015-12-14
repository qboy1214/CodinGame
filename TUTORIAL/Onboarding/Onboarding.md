### The Goal

Your program must destroy the enemy ships by shooting the closest enemy on each turn.

### Rules

Enemy ships always approach your cannon in a straight line.

**On each start of turn during the game** (within the game loop), you'll obtain information on the two closest enemies:

 - The variable enemy1: the name of enemy 1.
 - The variable dist1: the distance between your cannon and enemy 1.
 - The variable enemy2: the name of enemy 2.
 - The variable dist2: the distance between your cannon and enemy 2.

**Before your turn is over** (end of the loop), you must output the name of the closest enemy to make your cannon shoot it. In order to print the name of the closest enemy, you must use the variable enemy1 or enemy2.

### Pseudo Code Algorithm

To succeed in your mission, write the following algorithm (the grey blocks are already provided in the code editor, the red block must be removed from the code and the green blocks must be added):
```python
while true
	read enemy1
	read dist1
	read enemy2
	read dist2
	#print "name of the enemy"
	if dist1 is smaller than dist2
		print enemy1
	else
		print enemy2
	end if
end while
```