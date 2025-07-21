# Maze-Game
I created this maze game as an assignment for Accelerated Fundamentals of Computer Science 2. A random maze is generated using Kruskal's algorithm, and they are solved through breadth-first search (BFS), depth-first search (DFS), or manual movement. The creation and solving of the maze are animated, and all functionality works on both square and hexagonal mazes (see demo below). 

Please contact me directly to view the source code.

Here's how the program works:

## Maze + Kruskal's ##
The maze is constructed by assigning random weights to edges, sorting them from lowest -> highest weight, and then using union-find to create a minimum spanning tree. This process will iterate through every edge from lowest to highest weight and include them in the final maze if they do not form a cycle. This way, a random maze is created.

## Automatic Solution (BFS + DFS) ##
Users can use BFS or DFS to solve the maze, where both approaches are animated. Every cell in the maze that has been explored will change to light blue, and the final solution path will be traced back in dark blue. 

## Manual Solution (User movement) ##
Users can also manually solve the maze, using arrow keys to navigate through the maze. Every searched cell will appear light blue and, once they solve the maze, the shortest solution path will be traced back in dark blue. 

## Other Features ##
- once the program is launched, maze construction will be animated by tearing down 1 wall at a time

	- "n" - generate a completely new square maze
	- "t" - generate a completely new hexagonal maze

	- "v" - to create a new maze with vertical bias (using whatever is the current cell shape (square/hex))
	- "h" - to create a new maze with horizontal bias (using whatever is the current cell shape (square/hex))
   
	- "r" - to reset the current maze without producing a new maze
	
	- "s" - to run a DFS search on the current maze
	- "b" - to run a BFS search on the current maze
   
	- "g" - to render a gradient based on each node's distance to the target node (press again to toggle off)
	- "f" - to render a gradient based on each node's distance to the start node (press again to toggle off)
	
	- "m" - to enter manual mode
	- arrow keys - to traverse a square-celled maze when in manual mode
	- "w", "e", "d", "x", "z", "a" - to traverse a hexagonal-celled maze when in manual mode
	
	- "p" - to toggle the viewing of visited paths on or off
	- "o" - to obliterate all of the walls at once (rather than waiting for the destruction of individual walls to finish)


 Watch the demo, which includes the order of features being shown!
 Click [here](https://youtu.be/OIgNwQZo7cg)

