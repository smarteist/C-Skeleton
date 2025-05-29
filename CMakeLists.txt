cmake_minimum_required(VERSION 3.10)
project(hello_world VERSION 1.0)

# Set C standard and flags
set(CMAKE_C_STANDARD 99)
set(CMAKE_C_STANDARD_REQUIRED True)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -Werror")

# Specify include directories (relative to project root)
include_directories(${PROJECT_SOURCE_DIR}/src)

# List source files with relative paths
set(SOURCES
    ${PROJECT_SOURCE_DIR}/src/main.c
    ${PROJECT_SOURCE_DIR}/src/hello_world.c
    ${PROJECT_SOURCE_DIR}/src/hello_world.h
)

# Create executable target
add_executable(hello_world ${SOURCES})
