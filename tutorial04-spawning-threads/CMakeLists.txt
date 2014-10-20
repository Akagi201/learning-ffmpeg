#
# @file CMakeLists.txt
# @author Akagi201
# @date 2014/10/10
#

cmake_minimum_required(VERSION 2.8.4)
project(spawning_threads)

set(SOURCE_FILES main.c)

include_directories("/usr/local/include")

link_directories("/usr/local/lib")

add_executable(spawning_threads ${SOURCE_FILES})

target_link_libraries(spawning_threads "libavformat.a" "libavcodec.a" "libavutil.a" "libswscale.a" "libSDL.a")
