cmake_minimum_required(VERSION 3.10.0)
 project(basics_02)

 # Make the header files visible to the project
 include_directories(include)

 # Manully add the source files using the `set` function
 # set(SOURCES src/main.c src/myFuncs.c)

 # use wildcard variable with file function to set the `SOURCE` variable
 file(GLOB SOURCES "src/*.c")

 add_executable(app ${SOURCES})
