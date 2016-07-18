cmake_minimum_required (VERSION 2.6)
project (final)
file(GLOB SRC_FILES *.cpp http-parser/http_parser.c)

add_executable(final ${SRC_FILES})

set(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
<<<<<<< HEAD
set(CMAKE_CXX_FLAGS  "-Wall -std=c++11 -L/usr/local/lib -L/usr/lib -luv")
=======
>>>>>>> 3a040c5800cd6c6d5499c9df68828256672c868e
TARGET_LINK_LIBRARIES(final uv)
