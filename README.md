# A--path-finding-using-Javascript

A* Pathfinding Visualization

This is my first attempt at A* pathfinding. I made this visualization to show the beauty of pathfinding. You can modify all major features of my algorithm through the graphics interface. Here I will go through the major features of my program.


To represent the map, the program uses a grid of nodes, in which each node has up to four traversable edges: up, down, left and right. One node is designated the root node, and another the target node. In addition, a node can be marked as impassable, effectively creating an obstacle around which an algorithm must navigate

go to the JavaScript file and you can customize starting and ending points, inorder to change the obstacle the frequency change the random value of input from anywhere between 0.1(minimum obstacles) to 0.9(maximum bastacle)


![nodes](https://user-images.githubusercontent.com/40710016/60679602-ceede380-9ea5-11e9-97ec-ec3dfbdbf311.png)






Evaluating a node involves first checking if it is the target node – if this is the case, a path has been found and the algorithm terminates. Failing this, the node is removed from the open set and marked as visited so that is will not be re-added (this prevents the algorithm from generating loops). Finally, each of the nodes immediate unvisited neighbours are added to the open set. Crucially, for each of these neighbouring nodes, the current node is marked as their predecessor.


how to change the starting and ending node

![startend](https://user-images.githubusercontent.com/40710016/60679844-bfbb6580-9ea6-11e9-9cee-649499df4fd9.PNG)



In order to generate a path, each algorithm utilises an open set, a collection of nodes representing the boundary of an increasing search area. The algorithm gradually expands the search area by evaluating one node at a time from its open set.
