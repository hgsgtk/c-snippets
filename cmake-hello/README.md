# CMake Hello World

https://github.com/jameskbride/cmake-hello-world

## build and install

```
$ mkdir build
$ cd build

$ cmake ..
-- The C compiler identification is AppleClang 12.0.0.12000032
-- The CXX compiler identification is AppleClang 12.0.0.12000032
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /Library/Developer/CommandLineTools/usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /Library/Developer/CommandLineTools/usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Configuring done
-- Generating done
-- Build files have been written to: /Users/{user}/src/github.com/hgsgtk/c-snippets/cmake-hello/build

$ make
[ 50%] Built target Hello
Scanning dependencies of target CMakeHelloWorld
[ 75%] Building CXX object CMakeFiles/CMakeHelloWorld.dir/HelloWorld.cpp.o
[100%] Linking CXX executable CMakeHelloWorld
[100%] Built target CMakeHelloWorld

$ make install
[ 50%] Built target Hello
[100%] Built target CMakeHelloWorld
Install the project...
-- Install configuration: ""
-- Installing: /usr/local/bin/libHello.a
-- Installing: /usr/local/include/Speaker.h
-- Installing: /usr/local/bin/CMakeHelloWorld
```

## cleanup

```
rm /usr/local/bin/libHello.a /usr/local/include/Speaker.h /usr/local/bin/CMakeHelloWorld
```
