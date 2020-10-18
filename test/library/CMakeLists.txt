# library test build file for App

# standalone library testing
if(NOT PROJECT_NAME)
    cmake_minimum_required(VERSION 3.18.4)
    project(AppTestLibrary)
    enable_testing()

    # @TODO Setup for standalone library testing
endif()

# @TODO Setup library tests
add_test(NAME test_library COMMAND ${CMAKE_CURRENT_SOURCE_DIR}/test_library.sh)
