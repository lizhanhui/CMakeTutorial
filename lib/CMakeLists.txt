cmake_minimum_required(VERSION 3.2)
project("lib")

set(LIB_SOURCE_FILES hello.h hello.cpp)

# shared library
add_library(lib SHARED ${LIB_SOURCE_FILES})

# static library
# add_library(lib ${LIB_SOURCE_FILES})

set(LIBRARY_OUTPUT_PATH  ${PROJECT_BINARY_DIR}/lib)

# rename library name
set_target_properties(lib PROPERTIES OUTPUT_NAME "hello")