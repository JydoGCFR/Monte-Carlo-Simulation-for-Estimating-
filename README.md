# **Monte Carlo Simulation for Estimating π**

**Objective**

The objective of this project is to estimate the value of π using the Monte Carlo simulation technique. This method utilizes random numbers to simulate the process of throwing darts at a square board containing an inscribed quarter-circle. By counting how many darts land inside the circle versus how many are thrown, we can approximate the value of π.

**Methodology**
**Random Coordinate Generation:**

Used NumPy to generate random uniform numbers representing the x and y coordinates of darts thrown within the first quadrant of the unit square. The random numbers were generated in the range [0, 1].
The random seed was set to 12345 for reproducibility.
**Distance Calculation:**
For each dart, the distance from the origin (0, 0) was calculated.​
 
A dart is considered to be inside the quarter-circle if its distance from the origin is less than or equal to 1.
Counting Successful Darts:

A boolean array was created to determine which darts landed inside the quarter-circle.
The number of successful darts (those inside the circle) was counted.

**Estimating π:**

The estimate for π was also calculated .
This estimate leverages the ratio of the area of the quarter-circle to the area of the unit square.

**Visualization:**

A scatter plot was generated using Matplotlib to visually represent the coordinates of the darts, with distinct colors for those inside and outside the quarter-circle.

**Summary**

Using the NumPy library enabled efficient generation of random coordinates and streamlined the calculations needed for the Monte Carlo simulation. The simulation was conducted with a total of 1,000,000 darts, leading to an estimated value of π based on the proportion of darts that landed inside the quarter-circle.

The visualization created with Matplotlib effectively demonstrated the distribution of darts, clearly showing the area within the quarter-circle compared to the entire unit square. This project illustrates the power of simulation techniques in estimating mathematical constants and provides an engaging visual representation of the underlying processes.
