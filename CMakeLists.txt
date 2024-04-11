cmake_minimum_required(VERSION 3.26)  # CMake version check
project(cpptest)               # Create project "cpptest"
set(CMAKE_CXX_STANDARD 23)            # Enable c++23 standard

# Add test.cpp file of project root directory as source file
set(SOURCE_FILES test.cpp)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_compile_definitions(_XOPEN_SOURCE)

# Add executable target with source files listed in SOURCE_FILES variable
add_executable(cpptest ${SOURCE_FILES})