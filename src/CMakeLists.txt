cmake_minimum_required(VERSION 3.28.1)
project(demo VERSION 1.0)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)
add_executable(${PROJECT_NAME} main.cpp)
configure_file(${PROJECT_NAME}.h.in ${PROJECT_NAME}.h)
target_include_directories(${PROJECT_NAME} PUBLIC "${PROJECT_BINARY_DIR}")
