# Set global variables
cmake_minimum_required(VERSION 2.8)
project(ev3-autopilot)

# Set compiler parameters
set(CMAKE_C_FLAGS "-Wall -Wextra")
set(CMAKE_C_FLAGS_DEBUG "-g -O")
set(CMAKE_C_FLAGS_RELEASE "-O")

# Set CMake parameters
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/../install/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/../install/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/../install/bin)

# Set include directories
include_directories(include)

# Add subdirectories
add_subdirectory(src)
