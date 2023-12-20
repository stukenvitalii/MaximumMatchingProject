cmake_minimum_required(VERSION 3.27)
project(CourseProject)

MATH(EXPR stack_size "16 * 1024 * 1024") # 16 Mb
set(CMAKE_EXE_LINKER_FLAGS "-Wl,--stack,${stack_size}")

set(CMAKE_CXX_STANDARD 20)

add_executable(CourseProject main.cpp)
