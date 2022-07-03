cmake_minimum_required(VERSION 3.22)
project(getVideo C)

set(CMAKE_C_STANDARD 99)

include_directories(./include/)
link_directories(./libs/)
add_executable(getVideo main.c)

target_link_libraries(getVideo
        avcodec
        avdevice
        avfilter
        avformat
        avutil
        swresample
        swscale
        )
