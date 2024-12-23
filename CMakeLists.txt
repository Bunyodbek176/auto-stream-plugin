cmake_minimum_required(VERSION 3.10)

project(auto_stream_plugin)

set(OBS_DIR "C:/path/to/your/obs-studio")

include_directories(${OBS_DIR}/libobs)
include_directories(${OBS_DIR}/UI)

add_library(auto_stream_plugin MODULE main.cpp)
target_link_libraries(auto_stream_plugin obs)
