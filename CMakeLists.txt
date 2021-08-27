cmake_minimum_required(VERSION 3.0.0)
project(luo_test VERSION 0.1.0)

include(CTest)
include_directories(/usr/local/include)
# prefer to put all your include folders/files under it
link_directories(/usr/local/lib)
# prefer to put all your lib files under it
enable_testing()

add_executable(${PROJECT_NAME} main.cpp src/glad.c)
# combine .cpp with glad.c
target_link_libraries(${PROJECT_NAME} libglfw.dylib)

add_library(main main.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
