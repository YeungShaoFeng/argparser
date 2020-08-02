cmake_minimum_required(VERSION 2.4)
project(argparser)

set(CMAKE_CXX_STANDARD 14)

IF (CMAKE_SYSTEM_NAME MATCHES "Windows")
    set(CMAKE_EXE_LINKER_FLAGS -static)
ENDIF()

SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++0x")

add_executable(
        argparser
        src/main.cpp
)

INCLUDE_DIRECTORIES(
        include
)