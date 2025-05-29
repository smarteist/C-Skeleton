cmake_minimum_required(VERSION 3.10)

project(hello_world VERSION 1.0 LANGUAGES C)

# Language & warnings
set(CMAKE_C_STANDARD 99)
set(CMAKE_C_STANDARD_REQUIRED True)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -Werror")

# Specify include directories (relative to project root)
include_directories(${PROJECT_SOURCE_DIR}/src)

# Glob all .c and .h files in the src directory
file(GLOB_RECURSE SOURCES "src/*.c" "src/*.h")

add_executable(hello_world ${SOURCES})
