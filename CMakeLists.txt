cmake_minimum_required(VERSION 3.19)
project(d1)

add_executable(ttt "m.cpp")
add_subdirectory("d2")
message("${CMAKE_CURRENT_SOURCE_DIR}")
target_include_directories(ttt PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/d2")
target_link_libraries(ttt i)
