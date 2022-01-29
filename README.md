# Voyage-Into-the-unknown
Built Artificial Intelligence agents based on different variant of the robot path planning algorithm called Repeated A-star algorithm.

The algorithm for the repeated A-star is as follows:
1. Initialise the agent's initial position and the target location. Also, according to the agent's knowledge, the current grid contains all unblocked cells.
2. The agent does the following steps until it reaches the target:
   - The robot runs the A-star algorithm, on the current knowledge of the grid, which will find the shortest path that the agent will have to travel in the current knowledge of the grid to reach the target.
   - The robot starts travelling on the path and update it's knowldge as it travels on the new cells.
   - If the current cell of the path is unblocked, then the robot goes into the cell and updates it's knowledge
   - If the current cell of the path is blocked, then the robot will stop in the previous cell and update the knowledge. After updating it's knowledge, the robot will replan the from the current cell. 

#### In this project, we designed the variations of A-star algorithms for different situations. We explored 9 different situations which leads to 9 different algoritms.

## Agent 1
The initial location of the agent is top left corner of the grid and the target location is the botton right of the grid. The agent will implement the above described repeated A-star algorithm to find the shortest path from the start position to the target. In this project, the agent can sense cells into 8 different directions (N, S, E, W, NE, NW, SE, SW) and update it's knowledge.

## Agent 2

Similar to Agent 1, the inital location of the agent is the top left corne of the grid and the target location is the bottom right of the grid. The agent will be in the same situation as Agent 1 but this agent can look sense the cell that it is currently present on. So, here the agent will enter the next cell of the path and if it is unblocked it will update it's knowledge and continue and if the cell is blocked, then the agent will move back to the previous cell and replan the path using A-star algorithm.

For details and analysis of Agent 1 and Agent 2 algorithm refer to this [report]().
