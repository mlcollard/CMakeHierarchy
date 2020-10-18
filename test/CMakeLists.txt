# test build file for App

# Turn ON/OFF tests
option(BUILD_CLIENT_TESTS "Build client tests" ON)
option(BUILD_LIBRARY_TESTS "Build library tests" OFF)
option(BUILD_ALL_TESTS "Build all tests" OFF)

# standalone testing
if(NOT PROJECT_NAME)
    cmake_minimum_required(VERSION 3.18.4)
    project(AppTest)
    enable_testing()
    set(BUILD_ALL_TESTS ON)
endif()

# Turn ON building all tests
if(BUILD_ALL_TESTS)
    set(BUILD_CLIENT_TESTS ON)
    set(BUILD_LIBRARY_TESTS ON)
endif()

# @TODO Setup general test environment

if(BUILD_CLIENT_TESTS)
    add_subdirectory(client)
endif()

if(BUILD_LIBRARY_TESTS)
    add_subdirectory(library)
endif()
