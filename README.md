# maze-solving-robot-using-arduino
This code is for controlling a robot with two motors using 2 infrared sensors to detect black lines on the ground and adjust its movement accordingly to solve a given maze. 
Let's discuss how the robot can work and solve a maze using the provided code:

1. **Maze Solving Strategy:**
   - The robot will navigate through the maze by following the black lines on the ground.
   - At intersections, it will make decisions based on the sensor readings to determine the correct path to take.
   - The algorithm will involve turning left or right based on the availability of black lines detected by the sensors.

2. **Intersection Handling:**
   - When the robot encounters an intersection:
     - If both sensors detect black lines, it means there's a choice between turning left, right, or continuing straight.
     - The robot can implement various algorithms to make decisions at intersections, such as following a predefined rule like "always turn left" or "follow the right wall."
     - Once the decision is made, the robot will proceed in the chosen direction.

3. **Dead End Detection:**
   - If the robot reaches a dead end where both sensors detect a white surface (no black line), it needs to backtrack to the last intersection and choose a different path.
   - Backtracking can be achieved by implementing a stack or some form of memory to store previous decisions and backtrack accordingly.

4. **Speed Control and Stability:**
   - The robot's speed and stability are crucial for efficient maze-solving.
   - By adjusting the motor speeds dynamically based on sensor readings, the robot can maintain stability and navigate through the maze accurately.
   - The `MOTOR_SPEED` constant defined in the code can be adjusted to optimize the robot's speed for maze-solving.

5. **Testing and Optimization:**
   - Once the maze-solving algorithm is implemented, the robot can undergo testing in a maze environment.
   - During testing, observations can be made to fine-tune the algorithm and adjust parameters such as turning angles, speed thresholds, and intersection decision-making rules.

By following these principles and utilizing the provided code as a foundation, the robot can effectively navigate through a maze, making decisions at intersections and backtracking when necessary to find the optimal path to the maze's exit.
