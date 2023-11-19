cmake_minimum_required(VERSION 3.12)

project(GAMES101)

set(CMAKE_CXX_STANDARD 17)

add_subdirectory(00)
add_subdirectory(01)

install(TARGETS 00 01 DESTINATION output)
