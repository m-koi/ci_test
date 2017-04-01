cmake_minimum_required(VERSION 3.2)

project(ci_test)

find_package (OpenGL REQUIRED)
find_package (Bullet REQUIRED)

add_executable(app main.cpp)
