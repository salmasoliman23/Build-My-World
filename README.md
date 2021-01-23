# Build-My-World
This is the first project in the nanodegree program : Robotics Software Engineering from Udacity.
## Summary of Tasks

   - Build a single floor wall structure using the Building Editor tool in Gazebo. 
   - Model any object using the Model Editor tool in Gazebo. Model links should be connected with joints.
   - Import my structure and two instances of my model inside an empty Gazebo World.
   - Import at least one model from the Gazebo online library and implement it in my existing Gazebo world.
   - Write a C++ World Plugin to interact with my world. The code should display “Welcome to salma’s World!” message as soon as you launch the Gazebo world file.
   
## Directory Structure
      .Project1                             
       ├── my_Model                            # Model files 
       │   │   ├── model.config
       │   │   ├── model.sdf
       ├── scripts                             # Gazebo World plugin C++ script      
       │   ├── welcome.cpp
       ├── my_world                            # Gazebo main World containing models 
       │   ├── my.World
       ├── CMakeLists.txt               
       ├──  my_Building                        # Building files 
       │   │   ├── model.config
       │   │   ├── model.sdf
       ├── build                        
       │   │   ├── CMakeFiles
       │   │   ├── CMakeTmp
       │   │   ├── CMakeCache.txt
       │   │   ├── cmake_install.cmake
       │   │   ├── Makefile
       └── imgs
       
 ## To launch the simulation
 ###  Update and upgrade the Workspace
$ sudo apt-get update && sudo apt-get upgrade -y
 ### Clone the lab folder in /home/workspace/
- $ cd /home/workspace
- $ git clone https://github.com/salmasoliman23/Build-My-World/
### Compile the code
- $ mkdir build && cd build
- $ cmake ../
- $ make
### Add the library path to the Gazebo plugin path
$ export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:${PWD}
### Run the Gazebo World file
- $ gazebo my_World
