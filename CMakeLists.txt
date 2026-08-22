cmake_minimum_required(VERSION 3.15)

project(imgui LANGUAGES CXX)

add_library(imgui STATIC
        imgui.cpp
#        img_demo.cpp
        imgui_draw.cpp
        imgui_tables.cpp
        imgui_widgets.cpp
)

target_include_directories(imgui PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}
)