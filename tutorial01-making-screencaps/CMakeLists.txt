#
# @file CMakeLists.txt
# @author Akagi201
# @date 2014/10/10
#

cmake_minimum_required(VERSION 2.8.4)
project(making_screencaps)

set(SOURCE_FILES main.c)

include_directories("/usr/local/include")

link_directories("/usr/local/lib")

add_executable(making_screencaps ${SOURCE_FILES})

target_link_libraries(making_screencaps "libavformat.a" "libavcodec.a" "libavutil.a" "libswscale.a")
