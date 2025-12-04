cmake_minimum_required(VERSION 3.14)
project(zpp_bits)

add_library(${PROJECT_NAME} INTERFACE zpp_bits.h)
add_library(${PROJECT_NAME}::${PROJECT_NAME} ALIAS ${PROJECT_NAME})

target_compile_features(${PROJECT_NAME} INTERFACE cxx_std_20)
target_include_directories(${PROJECT_NAME} INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})
