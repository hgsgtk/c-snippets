cmake_minimum_required(VERSION 3.17)
project(cmakeHello)

set (CMakeHelloWorld_VERSION_MAJOR 1)
set (CMakeHelloWorld_VERSION_MINOR 0)

add_subdirectory(Hello)
include_directories(Hello)
add_executable(CMakeHelloWorld Hello HelloWorld.cpp)

target_link_libraries (CMakeHelloWorld Hello)

install (TARGETS CMakeHelloWorld DESTINATION bin)
