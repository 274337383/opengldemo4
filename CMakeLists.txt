cmake_minimum_required(VERSION 3.20)
project(opengldemo4)

set(CMAKE_C_STANDARD 11)

INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR}/include)
link_directories(${PROJECT_SOURCE_DIR}/lib)

add_executable(opengldemo4 main.cpp glad.c test.c)

target_link_libraries(opengldemo4 ${PROJECT_SOURCE_DIR}/lib/glfw3.dll)
