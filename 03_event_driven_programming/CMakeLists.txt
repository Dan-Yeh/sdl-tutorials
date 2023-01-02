cmake_minimum_required(VERSION 3.0)
project(mygame)


find_package(SDL2 REQUIRED COMPONENTS SDL2)

# Create your game executable target as usual 
add_executable(mygame 03_event_driven_programming.cpp)

# Link to the actual SDL2 library. 
target_link_libraries(mygame PRIVATE SDL2::SDL2)