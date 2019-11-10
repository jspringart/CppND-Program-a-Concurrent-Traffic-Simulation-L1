# CppND-Program-a-Concurrent-Traffic-Simulation-L1

Overview  
[![Alt text](https://img.youtube.com/vi/iifZEu0ctxc/0.jpg)](https://youtu.be/iifZEu0ctxc)

Code Walkthrough
Note: we recommend playing the video below full-screen so you will be able to see the code.  
[![Alt text](https://img.youtube.com/vi/OwiKpGYN9wI/0.jpg)](https://youtu.be/OwiKpGYN9wI)

Project Tasks
- **Task L1.1** : In the base class TrafficObject, set up a thread barrier in its destructor that ensures that all the thread objects in the member vector _threads are joined.
- **Task L1.2** : In the Vehicle class, start a thread with the member function drive and the object this as the launch parameters. Also, add the created thread into the _thread vector of the parent class.
- **Task L1.3** : Vary the number of simulated vehicles in main and use the top function on the terminal or the task manager of your system to observe the number of threads used by the simulation.
You can find these tasks in the project_tasks.txt within the workspace as well.

Build Instructions
To run this code using a Udacity workspace, you will need to use the virtual desktop. In the desktop you can use Terminator or the terminal in Visual Studio Code.

Once in the virtual desktop, to compile and run the code, create a build directory and use cmake and make as follows:

root@a9ad274128c4:/home/workspace/L1_Project# mkdir build  
root@a9ad274128c4:/home/workspace/L1_Project# cd build  
root@a9ad274128c4:/home/workspace/L1_Project/build# cmake ..  
root@a9ad274128c4:/home/workspace/L1_Project/build# make  
root@a9ad274128c4:/home/workspace/L1_Project/build# ./traffic_simulation  


## Dependencies for Running Locally
* cmake >= 2.8
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* OpenCV >= 4.1
  * The OpenCV 4.1.0 source code can be found [here](https://github.com/opencv/opencv/tree/4.1.0)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory in the top level directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./traffic_simulation`.

