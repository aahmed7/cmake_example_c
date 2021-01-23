cmake_minimum_required(VERSION 3.11...3.19)

project(
    CMake_Example
    VERSION 1.0
    LANGUAGES C
)

# Include headers(*.h) into the project.
include_directories(include)

# Include the source files(*.c) into the project.
file(GLOB SOURCES "src/*.c")

# Create a buildable target.
add_executable(testprint ${SOURCES})