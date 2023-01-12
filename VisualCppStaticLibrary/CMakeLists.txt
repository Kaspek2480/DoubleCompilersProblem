cmake_minimum_required(VERSION 3.0)
project(mylibrary)

# Add the source files for the library
add_library(mylibrary STATIC mylibrary.c mylibrary.h)
# Add the header files for the library
target_include_directories(mylibrary PRIVATE include)