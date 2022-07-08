cmake_minimum_required(VERSION 3.17)

project("skype-clients" VERSION 0.0.1 LANGUAGES CXX)

###############################################################################
# BUILD PROJECT
###############################################################################

set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR}/../)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)

set(CMAKE_CXX_FLAGS_DEBUG "${CMAKE_CXX_FLAGS_DEBUG} -ggdb3")
set(CMAKE_CXX_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE} -O3")

set(PROJECT_SOURCES
    )

add_executable(${PROJECT_NAME}
    src/Main.cpp
    ${PROJECT_SOURCES}
    )

target_include_directories(
    ${PROJECT_NAME}
    PRIVATE
    include/
    )
