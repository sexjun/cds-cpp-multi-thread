cmake_minimum_required(VERSION 3.0.0)
project(cpp_muti VERSION 0.1.0)

include(CTest)
enable_testing()

include_directories(./include)
aux_source_directory(SRC src)
add_executable(cpp_muti ${SRC} main.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
