cmake_minimum_required(VERSION 3.12)

# /usr/local
# message(${CMAKE_INSTALL_PREFIX})
# /home/shenyue/Projects/games101
# message(${CMAKE_HOME_DIRECTORY})

project(GAMES101)

set(CMAKE_CXX_STANDARD 17)
set(OUTPUT_DIRECTORY ${CMAKE_HOME_DIRECTORY}/output)


add_subdirectory(00)
add_subdirectory(01)
add_subdirectory(02)
add_subdirectory(03)

install(TARGETS 00 01 02 03 DESTINATION ${OUTPUT_DIRECTORY})
install(DIRECTORY 03/models DESTINATION ${OUTPUT_DIRECTORY})
