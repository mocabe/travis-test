cmake_minimum_required(VERSION 2.8)
enable_testing()
project(travis-test)

set(CMAKE_CXX_FLAGS "-std=c++14 -Wall")
include_directories("${PROJECT_SOURCE_DIR}")

add_subdirectory(src)
add_subdirectory(test)