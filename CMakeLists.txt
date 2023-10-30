# Minimum version of CMake required
cmake_minimum_required(VERSION 3.27)

include_directories(include)

link_directories(lib)

# Project name
project(sfml)

# Add the source file to the project
add_executable(main main.cpp)

# Link with SFML libraries
target_link_libraries(main PRIVATE sfml-graphics sfml-window sfml-system)
