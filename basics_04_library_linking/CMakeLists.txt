cmake_minimum_required(VERSION 3.10.0)
project(basics_04_library_linking)
# specify the production type
set(CMAKE_BUILD_TYPE Debug)

set(PROJECT_LINK_LIBS mathFuncs.a)
link_directories( ~/Documents/learning/tutorials_github/cmake/basics_03_library/build)
include_directories(~/Documents/learning/tutorials_github/cmake/basics_03_library/include)

add_executable(app src/main.c)
target_link_libraries(app ${PROJECT_LINK_LIBS})
