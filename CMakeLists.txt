# Master build file for App

cmake_minimum_required(VERSION 3.18.4)

project(App)

# must be at top-level
enable_testing()

add_subdirectory(src)
add_subdirectory(test)
