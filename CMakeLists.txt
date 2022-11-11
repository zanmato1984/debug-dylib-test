cmake_minimum_required(VERSION 3.23)

project(debug_dylib_test)

set(CMAKE_CXX_STANDARD 20)

add_library(foo SHARED foo.cpp)

add_executable(debug-dylib-test main.cpp)

target_link_libraries(debug-dylib-test foo)
