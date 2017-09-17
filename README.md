# Autonomous-Polynomial-Trajectory-Generation-Udacity
Polynomial Trajectory Generation Playground code from Udacity (SDCND)

Getting Started
From the project's directory, run python evaluate_ptg.py. You should see a plot. This plot shows the s (x-axis) and d(y-axis) trajectories followed by a vehicle in traffic (red) and a self driving car (blue).

In this situation, the self driving car was trying to get behind the target vehicle, but the cost functions it was using weren't weighted appropriately and so it didn't behave as expected.

Fixing the Problem(s)
There are 5 files in the provided code. You'll probably want to start by modifying cost function weights in ptg.py but may also want to add cost functions of your own. As a bonus challenge try implementing this same code in C++.

File Descriptions

ptg.py - The primary code for generating a polynomial trajectory for some constraints. This is also where weights are assigned to cost functions. Adjusting these weights (and possibly adding new cost functions), can have a big effect on vehicle behavior.
cost_functions.py - This file contains many cost functions which are used in ptg.py when selecting the best trajectory. Some cost functions aren't yet implemented...
evaluate_ptg.py - This file sets a start state, goal, and traffic conditions and runs the PTG code. Feel free to modify the goal, add traffic, etc... to test your vehicle's trajectory generation ability.
constants.py - constants like speed limit, vehicle size, etc...
helpers.py - helper functions used by other files.
