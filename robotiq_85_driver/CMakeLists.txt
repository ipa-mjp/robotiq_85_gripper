cmake_minimum_required(VERSION 2.8.3)
project(robotiq_85_driver)

find_package(catkin REQUIRED)

## Uncomment if the package has a setup.py
catkin_python_setup()

find_package(catkin REQUIRED COMPONENTS roslaunch rospy)

catkin_package()

catkin_install_python(PROGRAMS bin/robotiq_85_driver bin/robotiq_85_test bin/robotiq_85_action_server bin/robotiq_85_action_client_example
                      DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})
                      
