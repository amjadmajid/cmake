The `include_directories()` function is used to bring the header files into the building environment. 
The `set( VARIABLE ...)` function is used to set a variable. 
The `file()` command is used to add the source files to the project. 
The `GLOB` is used to expnad the wildcard `*` to match anything. 
The ${VARIABLE}` is used to dereference the vaiable. 

### To build the project
1. `mkdir build`
2. `cd build`
3. `cmake ..` (the cmake needs to be run on the top level CMakeLists.txt)
4. make (cmake will generate a Makefile and the make will build the target)
