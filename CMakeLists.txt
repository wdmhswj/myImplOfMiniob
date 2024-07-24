cmake_minimum_required(VERSION 3.10)    # cmake版本要求
set(CMAKE_CXX_STANDARD 20)  # c++版本要求

project(myImplOfMiniob) # 项目名

MESSAGE(STATUS "This is Project source dir " ${PROJECT_SOURCE_DIR})
MESSAGE(STATUS "This is PROJCET_BINARY_DIR dir " ${PROJECT_BINARY_DIR})

SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)   # 设置可执行文件目录

# 更新 CMAKE_MODULE_PATH 变量，使其包含当前项目源目录下的 cmake 子目录
SET(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} ${CMAKE_SOURCE_DIR}/cmake)

