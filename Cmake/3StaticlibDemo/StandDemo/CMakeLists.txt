# Cmake最低版本
cmake_minimum_required(VERSION 3.10)
# 定义工程名称
project(StandDemo VERSION 1.0.0)

# 设置C++标准
set(CMKAE_CXX_STANDRD 11)
set((CMKAE_CXX_STANDRD_REQUIRED ON)

# 添加头文件搜索路径
include_directories(${PROJECT_SOURCE_DIR}/include)

# 源文件
aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR}/src SRC_LIST)

add_executable(StandDemo ${SRC_LIST} main.cpp)