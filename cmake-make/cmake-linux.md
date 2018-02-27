### Cmake Project Build
* Let There is a Project Folder
* Folder Contents
#### CMakeLists.txt
```cmake
cmake_minimum_required(VERSION 2.8)

project(Main)
add_executable(${PROJECT_NAME} "main.cpp")
```
### main.cpp
```cc
#include <iostream>

using namespace std;

int main()
{
    int n = 0;
    cin >> n;
    for(int i = 0; i <= n; i++)
    cout << "I am in line Number: " << i << endl;
    return 0;
}
```
* Make a directory called ` build ` in current directory
```sh
mkdir build
cd build
```

* Now create make file using ` cmake ..` command
* Or You can specify compiler
```sh
cmake -D CMAKE_C_COMPILER=/usr/bin/gcc-7 ..
```

* Now build project using ` make ` command
* Or You can specify compiler
```sh
make CC=/usr/bin/gcc-7
```
