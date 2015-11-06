cmake_minimum_required(VERSION 3.2)
project("lib")

set(LIB_SOURCE_FILES hello.h hello.cpp)

add_library(lib ${LIB_SOURCE_FILES})

set(LIBRARY_OUTPUT_PATH  ${PROJECT_BINARY_DIR}/lib)