# Try build by cmake

ref: https://qiita.com/shohirose/items/45fb49c6b429e8b204ac

## build by g++

- ソースファイルをcompile、オブジェクトファイルへ

```
g++ -c main.cpp hello.cpp
```

- オブジェクトファイルをリンク、実行ファイルを生成

```
g++ -o a.out main.o hello.o
```

- 直接ソースファイルから実行ファイルを作成する場合

```
g++ -o a.out main.cpp hello.cpp
```

## build by cmake

https://cmake.org/download/ からlatestをinstallする手もあるが、Homebrewがお手軽。

```
brew install cmake
```

<!-- ref: https://qiita.com/kai_kou/items/df335eb7ee78229ee46f -->

```
$ cmake --version
cmake version 3.19.1

CMake suite maintained and supported by Kitware (kitware.com/cmake).
```

- 実行ファイル生成 by make

```
$ cd build
$ cmake ..
cmake ..
-- Configuring done
-- Generating done
-- Build files have been written to: /Users/{user}/src/github.com/hgsgtk/c-snippets/try-cmake/build
$ make
```

## Trouble Shooting

- build failure while making by cmake

```
$ make
[ 50%] Linking CXX executable main.cpp
Undefined symbols for architecture x86_64:
  "_main", referenced from:
     implicit entry/start for main executable
ld: symbol(s) not found for architecture x86_64
clang: error: linker command failed with exit code 1 (use -v to see invocation)
make[2]: *** [main.cpp] Error 1
make[1]: *** [CMakeFiles/main.cpp.dir/all] Error 2
make: *** [all] Error 2
```

https://marycore.jp/prog/xcode/undefined-symbols-for-architecture-x86-64/



