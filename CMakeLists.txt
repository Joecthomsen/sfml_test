cmake_minimum_required(VERSION 3.16.3)
project(my_project)

add_executable(${PROJECT_NAME} main.cpp)

add_subdirectory(external/sfml/)

target_include_directories(${PROJECT_NAME} PUBLIC external/sfml/include)
target_link_directories(${PROJECT_NAME} PUBLIC external/sfml/src)

