cmake_minimum_required(VERSION 3.16.3)
project(MY_PROJECT)

add_executable(${PROJECT_NAME} main.cpp)

#add_subdirectory(external/include)

target_include_directories(${PROJECT_NAME} PUBLIC external/include)

target_link_directories(${PROJECT_NAME} PUBLIC external/lib)

target_link_libraries(${PROJECT_NAME} libsfml-audio.so libsfml-graphics.so sfml-system libsfml-window.so)