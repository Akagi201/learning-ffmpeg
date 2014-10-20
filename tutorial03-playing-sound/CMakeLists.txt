#
# @file CMakeLists.txt
# @author Akagi201
# @date 2014/10/10
#

cmake_minimum_required(VERSION 2.8.4)
project(playing_sound)

set(SOURCE_FILES main.c)

include_directories("/usr/local/include")

link_directories("/usr/local/lib")

add_executable(playing_sound ${SOURCE_FILES})

target_link_libraries(playing_sound "libavformat.a" "libavcodec.a" "libavutil.a" "libswscale.a" "libSDL.a")
