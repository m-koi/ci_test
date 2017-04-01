cmake_minimum_required(VERSION 3.2)

project(ci_test)

find_package (OpenGL REQUIRED)
find_package (Bullet REQUIRED)

add_subdirectory(${PROJECT_SOURCE_DIR}/ext/glfw)

include_directories (${PROJECT_SOURCE_DIR}/ext/glfw/include)

add_executable(app main.cpp)
target_link_libraries(app glfw ${OPENGL_LIBRARY})
