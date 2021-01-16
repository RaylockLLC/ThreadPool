cmake_minimum_required (VERSION 3.16)

project(mvThreadPool)

find_package(Threads)
add_executable(${PROJECT_NAME} "main.cpp")
target_link_libraries( ${PROJECT_NAME} ${CMAKE_THREAD_LIBS_INIT} )
set_property(TARGET ${PROJECT_NAME} PROPERTY CXX_STANDARD 17)
