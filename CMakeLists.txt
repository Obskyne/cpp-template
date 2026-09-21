cmake_minimum_required(VERSION 3.23)
project(MyProject CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_BUILD_TYPE Debug)

# Target executable
add_executable(${PROJECT_NAME} Source/main.cpp)

# Link Include directory natively
target_include_directories(${PROJECT_NAME} PUBLIC Include)
