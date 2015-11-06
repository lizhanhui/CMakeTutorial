cmake_minimum_required(VERSION 3.2)
project(CMakeTutorial)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

add_subdirectory(lib)
add_subdirectory(app)