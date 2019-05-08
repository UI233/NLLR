cmake_minimum_required(VERSION 3.0)
set(CMAKE_BUILD_TYPE "Release")
project(NLLR)
set(CMAKE_CXX_STANDARD 11)
# set(CMAKE_CXX_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE} -O3")

include_directories(${CMAKE_CURRENT_SOURCE_DIR})
# get all *.cpp files recursively
file(GLOB_RECURSE SRC_FILES mesh/*.cpp)

add_executable(NLLR meshviewer.cpp ${SRC_FILES})
