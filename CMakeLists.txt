#
#  CMakeLists.txt
#  miniaudio
#
#  Created by Dmitrii Torkhov <dmitriitorkhov@gmail.com> on 15.08.2021.
#  Copyright © 2021 Dmitrii Torkhov. All rights reserved.
#

cmake_minimum_required(VERSION 3.14 FATAL_ERROR)

project(miniaudio
        VERSION 0.10.41
        LANGUAGES C)

#

add_library(miniaudio INTERFACE
        miniaudio.h)

target_include_directories(miniaudio INTERFACE
        $<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}>)