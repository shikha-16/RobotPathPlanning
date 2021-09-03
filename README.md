# Robot Path Planning
The robotic path planning problem is a classic. A robot is attempting to navigate its path from the start point to a specified goal region, while avoiding the set of all obstacles.

## Rapidly exploring Random Trees
In RRT, points are randomly generated within a specified radius and connected to the nearest existing node. Each time a node is created, we check that it lies outside of the obstacles. Furthermore, chaining the node to its closest neighbor must also avoid obstacles. The algorithm ends when a node is generated within the goal region, or a limit is hit. RRT* is an optimized version of RRT. When the number of nodes approaches infinity, the RRT* algorithm will deliver the shortest possible path to the goal. 
