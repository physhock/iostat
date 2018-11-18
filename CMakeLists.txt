cmake_minimum_required(VERSION 3.12)
project(iostat C)

set(CMAKE_C_STANDARD 11)
set(HEADERS headers/version.h headers/sysconfig.h headers/iostat.h)

add_executable(iostat iostat.c ${HEADERS})
include_directories(library)
add_subdirectory(library)
target_link_libraries(iostat lib)