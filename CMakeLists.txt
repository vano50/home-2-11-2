cmake_minimum_required(VERSION 3.30)
project(home-2-11-3 VERSION 0.1 LANGUAGES CXX)
set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY /run)
add_library(Leaver SHARED Leaver.h Leaver.cpp)
add_executable(home-2-11-3 main.cpp)
target_link_libraries(home-2-11-3 Leaver)
