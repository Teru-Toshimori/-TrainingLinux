cmake_minimum_required(VERSION 3.16)

project(SensorAnalyzer C)

set(CMAKE_C_STANDARD 17)
set(CMAKE_C_STANDARD_REQUIRED ON)

add_subdirectory(lib)
add_subdirectory(app)
