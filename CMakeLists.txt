cmake_minimum_required(VERSION 3.16)
project(iconvlite)

add_library(${PROJECT_NAME} STATIC iconvlite.cpp)
target_include_directories(${PROJECT_NAME} PUBLIC .)

add_executable(${PROJECT_NAME}-example example.cpp)
target_link_libraries(${PROJECT_NAME}-example ${PROJECT_NAME})