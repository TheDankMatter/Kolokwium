cmake_minimum_required(VERSION 3.1)
project(myProgram)

file(GLOB SOURCES src/*.cpp)
add_executable(myProgram ${SOURCES})