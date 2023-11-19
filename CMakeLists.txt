cmake_minimum_required(VERSION 3.12)

project(GAMES101)

set(CMAKE_CXX_STANDARD 17)
set(Eigen3_DIR  /usr/local/include/eigen3)

add_subdirectory(00)

install(TARGETS 00 DESTINATION output)
