cmake_minimum_required(VERSION 3.8)
set(CMAKE_CXX_STANDARD 11)
set(PROJECT_NAME g13_schneller)
project(${PROJECT_NAME})

include_directories(src)
add_subdirectory(src)

target_include_directories(g13_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

add_executable(${CMAKE_PROJECT_NAME} src/g13.cc)