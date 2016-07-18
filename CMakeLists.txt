cmake_minimum_required (VERSION 2.6)
project (final)
file(GLOB SRC_FILES *.cpp http-parser/http_parser.c)

add_executable(final ${SRC_FILES})

set(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
set(CMAKE_CXX_FLAGS  "-Wall -std=c++11 -L/usr/local/lib -L/usr/lib -luv")
TARGET_LINK_LIBRARIES(final uv)
