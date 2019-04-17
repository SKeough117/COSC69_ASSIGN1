Sean Keough
COSC 69: Multi-Robot Systems
Professor Alberto Quattrini Li
Spring 2019


This document will contain instructions for properly running my flocking package. Fair warning, this is my first time ever
sending a package and using a .zip file to do so, so I hope that it works well.

1. Download and Unzip the SKeough_COSC69_Assign1 file

2. Place the file (flock_code) within your catkin workspace within Ubuntu, placing it within the source folder

3. First, open up terminal (every terminal you open, start with '$ source devel/setup.bash') and ensure that your log files
are cleared (I had to do this in order for the program to work) ==> $ rosclean purge

4. After, start up your roscore

5. Open a secondary terminal, and launch the simulation file with the following command:
  - $ roslaunch $(rospack find flock_code) simulation.launch
  
6. This should immediately initialize all the robots and the stage, and call the flock function on an infinite loop,
continuously calling the robots to action. After a few seconds (depending on the speed of your computer), the stage should pop up and the robots will begin moving.

7. To restart the simulation, simply Control C the terminal running the simulation and relaunch the package

