cmake_minimum_required(VERSION 3.17)
project(VKCoreTest)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Werror -Wall -Wextra -Wpedantic")

include(CTest)
add_subdirectory(Test)
enable_testing()

add_executable(VKCoreTest main.cpp)
