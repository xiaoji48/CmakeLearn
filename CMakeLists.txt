cmake_minimum_required(VERSION 3.0)

project(SWAP)

# 获取源文件所在路径下的所有源文件列表
aux_source_directory(${PROJECT_SOURCE_DIR}/src SRC)

# 设置引用的头文件路劲
include_directories(${PROJECT_SOURCE_DIR}/include)

# 设置静态库或者动态库的输出路径
set(LIBRARY_OUTPUT_PATH /mnt/d/CodeField/CmakeTest/bin)

add_library(swap SHARED ${SRC})