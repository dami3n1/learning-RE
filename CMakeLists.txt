cmake_minimum_required(VERSION 3.10)

# Project name and version
project(MyProject VERSION 1.0 LANGUAGES CXX)

# C++ standard
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Optional: Set output directories
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

# Include directories
include_directories(include)

# Add source files
file(GLOB SOURCES "*.cpp")

# Add the executable
add_executable(${PROJECT_NAME} ${SOURCES})

