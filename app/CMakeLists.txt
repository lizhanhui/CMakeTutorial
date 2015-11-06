cmake_minimum_required(VERSION 3.2)
project(app)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

include_directories(../lib)

set(APP_SOURCE_FILES main.cpp)

add_executable(app ${APP_SOURCE_FILES})
target_link_libraries(app lib)

set(EXECUTABLE_OUTPUT_PATH  ${PROJECT_BINARY_DIR}/bin)