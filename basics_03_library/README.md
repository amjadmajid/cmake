Using the `add_library()` with `SHARED`/`STATIC` flag, enables cmake to generate a Makefile for a shared/static library <br>
The `install()` defines the installation location for the library. <br>
Note some installation locations might requie a _root_ privileges, i.e. /usr/lib.

### To build the shared library
1. `mkdir build && cd build`
2. `cmake ..`
3. `sudo make install`
