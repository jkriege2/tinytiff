cmake_minimum_required(VERSION 3.10)

project(extcmake_tinytiff_test CXX)

find_package(TinyTIFF)

add_executable(${PROJECT_NAME}
	extcmake_tinytiff_test.cpp
)

target_link_libraries(${PROJECT_NAME} TinyTIFF::TinyTIFF)
