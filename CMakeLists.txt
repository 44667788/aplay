cmake_minimum_required(VERSION 3.7)
project(wav)
#include_directories("/home/zeke/project/fiio_player/out/product/halley2/include/" )
set(CMAKE_C_STANDARD 99)

set(SOURCE_FILES aplay.c)
#SET(CMAKE_C_COMPILER /home/zeke/devTool/mips-gcc472-glibc216/bin/mips-linux-gnu-gcc)
#SET(CMAKE_CXX_COMPILER /home/zeke/devTool/mips-gcc472-glibc216/bin/mips-linux-gnu-g++)
#link_directories("/home/zeke/project/fiio_player/out/product/halley2/system/usr/lib"
#        "/home/zeke/project/fiio_player/out/product/halley2/system/lib")
add_executable(aplay ${SOURCE_FILES})
target_link_libraries(aplay asound rt)