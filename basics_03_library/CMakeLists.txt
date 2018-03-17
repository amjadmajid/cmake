cmake_minimum_required(VERSION 3.10.0)
project(basics_04_shared_library)
# specify the production type
set(CMAKE_BUILD_TYPE Release)

 # Make the header files visible to the project
 include_directories(include)

 # use wildcard variable with file function to set the `SOURCES` variable
 file(GLOB SOURCES "src/*.c")

 # Generate a shared library
 #add_library(mathFuncs SHARED ${SOURCES})

 # Generate a static library
  add_library(mathFuncs STATIC ${SOURCES})

 # set the library installation location, for example (/usr/lib)
 install (TARGETS mathFuncs DESTINATION /usr/local/lib)
