cmake_minimum_required(VERSION 2.6)
project(Correlation)
#set(CMAKE_C_FLAGS "-Wall -g")
set(CMAKE_CXX_FLAGS "-std=c++11 -g -Wall")

set(AP_VERSION 0.0.2)
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake/Modules/")
set(CMAKE_BUILD_TYPE Debug)

find_package(ROOT REQUIRED)
#find_package(cfitsio REQUIRED)
find_package(URAnalysis REQUIRED)
include_directories(${ROOT_INCLUDE_DIR})

#add_subdirectory(convert)
#add_subdirectory(createmock)
#add_subdirectory(correlation)
add_subdirectory(correlation_fast)

