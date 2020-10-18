# client test build file for App

# standalone client testing
if(NOT PROJECT_NAME)
    cmake_minimum_required(VERSION 3.18.4)
    project(AppTestClient NONE)
    enable_testing()

    # @TODO Setup for standalone client testing
endif()

# @TODO Setup client tests for app
add_test(NAME test_run COMMAND ${CMAKE_CURRENT_SOURCE_DIR}/test_run.sh)
