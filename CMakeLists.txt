

cmake_minimum_required(VERSION 3.22 FATAL_ERROR)
project(fredbuf LANGUAGES CXX)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_COMPILER g++-13)

add_library(fredbuf fredbuf.cpp)

add_executable(fredbuf-tests fredbuf-test.cpp)
target_link_libraries(fredbuf-tests PRIVATE fredbuf)