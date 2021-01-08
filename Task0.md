# TASK 0
This task is to create the workspace and get used to the directory structure. The basic terminal commands are highlighted clearly. The commands are sequential and in a do-along format for future reference.

## Steps 

1. Source the setup *sh file to get ROS functionality. This needs to be done for every new terminal unless the line has been added to .bashrc file. The \<distro> provides the option to have multiple ROS versions installed and switch between them.   
> $ source /opt/ros/\<distro>/setup.bash
2. Create the src folder inside another folder that will act as your workspace. The name of the workspace can be anything, subject to certain basic formatting rules. 
> $ mkdir -p ~/catkin_ws/src
3. Change directory to the workspace parent directory. 
> $ cd ~/catkin_ws
4. The catkin make command is to build the code in the workspace, any packages in the src folder. Read more about it [here](http://wiki.ros.org/catkin/commands/catkin_make). 
> $ catkin_make
5. Now there will be a devel and build folder along with the src folder that was created. To overlay this workspace on top of the environment we source one of the files in the devel folder.
> $ source devel/setup.bash
6. `CHECK` for proper overlay 
> $ echo $ROS_PACKAGE_PATH
> /home/youruser/catkin_ws/src:/opt/ros/kinetic/share

## Additional Reading
- [About workspaces](http://wiki.ros.org/catkin/workspaces)
- [Some basic commands](http://wiki.ros.org/ROS/Tutorials/NavigatingTheFilesystem)