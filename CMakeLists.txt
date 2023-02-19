cmake_minimum_required(VERSION 3.10)
project(my_project VERSION 1.0)

# Set compiler flags
set(CMAKE_C_STANDARD 99)
set(CMAKE_C_STANDARD_REQUIRED True)
set(CMAKE_C_FLAGS "-Wall -Werror")

# Add source files to project
set(SOURCES
        src/main.c
        # foo.c
        # bar.c
        src/hello_world.c src/hello_world.h)

# Add executable target
add_executable(my_program ${SOURCES})

