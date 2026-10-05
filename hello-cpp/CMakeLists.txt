cmake_minimum_required(VERSION 3.20)
project(hello-cpp LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(hello hello.cpp)

enable_testing()
add_test(NAME hello_runs COMMAND hello)
set_tests_properties(hello_runs PROPERTIES PASS_REGULAR_EXPRESSION "hello, world")
