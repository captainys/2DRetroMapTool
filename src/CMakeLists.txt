cmake_minimum_required(VERSION 3.2)
project(2DRetroMapTool)

if(EXISTS ${CMAKE_CURRENT_SOURCE_DIR}/../public)
	set(PUBLIC_SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/../public/src)
else()
	set(PUBLIC_SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/../../public/src)
endif()

add_subdirectory(${PUBLIC_SOURCE_DIR} ${CMAKE_BINARY_DIR}/public)
add_subdirectory(kernel)
add_subdirectory(kernel/gl2)
add_subdirectory(kernelutil)
add_subdirectory(gui)
