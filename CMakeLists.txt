cmake_minimum_required(VERSION 2.8)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -pthread -O3")

project(C++_template)

add_library(utils utils.cpp)

add_executable(main main.cpp)
target_link_libraries(main utils)