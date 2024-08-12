cmake_minimum_required(VERSION 3.13.4)

project(Bismillah)

add_executable(${PROJECT_NAME} main.cpp)

add_subdirectory(Adder)

# add include dir
target_include_directories(${PROJECT_NAME} PUBLIC Adder)

# 
target_link_directories(${PROJECT_NAME} PRIVATE Adder)

# link library to yr main
target_link_libraries(${PROJECT_NAME} adder)

