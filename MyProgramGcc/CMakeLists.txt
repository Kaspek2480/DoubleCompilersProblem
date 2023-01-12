add_executable(MyProgramGcc main.cpp)

cmake_minimum_required(VERSION 3.0)
set(CMAKE_VERBOSE_MAKEFILE ON)
project(myprogram)

set(CMAKE_CXX_STANDARD 17)

# Add the source files for the program
add_executable(myprogram main.cpp mylibrary.h)
# Add the include directories for the program
target_include_directories(myprogram PRIVATE include)
# Link the program with the library
target_link_libraries(myprogram -LC:/Users/Kaspek/CLionProjects/LinkerTest/VisualCppStaticLibrary/cmake-build-release-visual-studio -lmylibrary)
