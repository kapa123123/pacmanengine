cmake_minimum_required(VERSION 2.6)
project(PACMANENGINE)

include_directories(
 src
)

add_executable(demo
	src/demo/main.cpp
)


target_link_libraries(demo pacmanengine)

# h Files included to show in VS
add_library(pacmanengine SHARED
	src/pacmanengine/Core.cpp
	src/pacmanengine/Core.h
)
