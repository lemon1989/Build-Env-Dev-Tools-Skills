2020.12.12
-
CMake supports GDB debugging when compiled
-
In linux environment by setting the compilation option CXXFLAGS or CFLAGS so that the program can support GDB debugging,in the CMake construction project can also be convenient implementation.
-
Add the following statement to CMakeLists.txt file:
-
SET(CMAKE_BUILD_TYPE "Debug")
-
SET(CMAKE_CXX_FLAGS_DEBUG "$ENV{CXXFLAGS} -O0 -Wall -g2 -ggdb")
-
SET(CMAKE_CXX_FLAGS_RELEASE "$ENV{CXXFLAGS} -O3 -Wall")
-



