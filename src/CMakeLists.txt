cmake_minimum_required(VERSION 3.8)
set(CMAKE_CXX_STANDARD 11)

file(GLOB headers_ "*.h")
file(GLOB sources_ "*.cpp" "*.cc")

add_library(g13_lib ${headers_} ${sources_})

target_include_directories(g13_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})