The `include_directories()` function is used to bring the header files into the building environment. <br>
The `set( VARIABLE ...)` function is used to set a variable.<br> 
The `file()` command is used to add the source files to the project. <br>
The `GLOB` is used to expnad the wildcard `*` to match anything.<br> 
The `${VARIABLE}` is used to dereference the vaiable.<br> 

### To build the project
1. `mkdir build`
2. `cd build`
3. `cmake ..` (the cmake should be called against the top level CMakeLists.txt)
4. `make` (cmake will generate a Makefile and the make will build the target, using the generated Makefiles)
