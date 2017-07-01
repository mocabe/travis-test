cmake_minimum_required(VERSION 2.8)
enable_testing()
project(travis-test)

set(CMAKE_CXX_FLAGS "-std=c++14 -Wall")
add_subdirectory(test)