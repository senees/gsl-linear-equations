cmake_minimum_required(VERSION 3.22)

project(linear-equations C)

set(CMAKE_C_STANDARD 99)

add_executable(linear-equations main.c)

find_package(GSL REQUIRED)

target_link_libraries(linear-equations GSL::gsl GSL::gslcblas)