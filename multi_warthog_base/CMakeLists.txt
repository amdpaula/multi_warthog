cmake_minimum_required(VERSION 2.8.3)
project(multi_warthog_base)

find_package(catkin REQUIRED COMPONENTS roslaunch)

catkin_package()

roslaunch_add_file_check(launch/warthog_base.launch)

install(
	DIRECTORY launch
	DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
