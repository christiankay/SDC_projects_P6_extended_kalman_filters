# Extended-Kalman-Filter
Udacity CarND Term 2, Project 1 - Extended Kalman Filters

## Project Basics
In this project I utilized a kalman filter in C++ to estimate the state of a moving object of interest with noisy lidar and radar measurements. Passing the project required obtaining RMSE values that are lower than the tolerance outlined in the project rubric.

The code will make a prediction based on the sensor measurement and then update the expected position. See files in the 'src' folder for the primary C++ files making up this project.

## Build instructions
Assuming you have 'cmake' and 'make' already:
1. Clone this repo.
2. Make a build directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./ExtendedKF path/to/input.txt path/to/output.txt`. You can find some sample inputs in 'data/'.
    * eg. `./ExtendedKF ../data/sample-laser-radar-measurement-data-1.txt output.txt`

## Results
In two different simulated runs, my Extended Kalman Filter produces the below results. The x-position is shown as 'px', y-position as 'py', velocity in the x-direction is 'vx', while velocity in the y-direction is 'vy'. Residual error is calculated by mean squared error (MSE).

*Test Kalman Filter*

| Input |   MSE   |
| ----- | ------- |
|  px   | 0.06516 |
|  py   | 0.06054 |
|  vx   | 0.53321 |
|  vy   | 0.54419 |

![Test One Visualization](https://github.com/mvirgo/Extended-Kalman-Filter/blob/master/vis_1.png "Test One Visualization")



