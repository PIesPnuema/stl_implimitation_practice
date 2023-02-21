
stl_implimitation_practice
----

Recreating the std::containers and learning along the way

----

##### How to compile tests using CMake.
-----

I have included a empty build directory for to build for a place to build the tests.

1. from root directory cd into the build directory:
```bash
cd build
```
2. inside the build directory configure the project for your computer via the following command:
```bash
cmake ..
```
    - the ".." tell cmake the root CMakeLists.txt file to configure the project is back one directory.

3. build the project to obtain the executable. 
```bash
cmake --build . 
```
    - Here we are telling cmake to build the project in the current directory (build)

4. The executable is called STLPROJECT. To run the tests you just need to run the executable:
```bash
./STLPROJECT
```

If all configurations from UnitTest++ go well. All tests should pass.

----

##### Project File Structure

root_repo/
├── include/
│   ├── vector.    
│   ├── DList.h
│   └── ...
├── src/
│   ├── vector.cpp
│   ├── DList.cpp
│   └── ...
├── tests/
│   ├── main.cpp (runs all tests)
│   ├── vector_test.cpp
│   ├── DList_test.cpp
│   └── ...
├── CMakeLists.txt
└── build
