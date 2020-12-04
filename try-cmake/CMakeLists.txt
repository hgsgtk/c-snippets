cmake_minimum_required(VERSION 3.17)
project(hello_cmake CXX)
#add_executable(main.cpp hello.cpp)
add_executable(main.cpp ../cmake-hello/HelloWorld.cpp ../cmake-hello/HelloWorld.h ../cmake-hello/Hello/Speaker.cpp ../cmake-hello/Hello/Speaker.h)
