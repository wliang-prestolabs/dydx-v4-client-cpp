cmake_minimum_required(VERSION 3.11)

project(dydx_v4_client
        VERSION 0.0.1
        LANGUAGES CXX
        DESCRIPTION "dYdX v4 client for C++"
)

set(CMAKE_CXX_STANDARD 17)
set(warnings "-Wall -Wextra")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${warnings}")

set(INCLUDE_DIR include)
set(SOURCE_DIR src)

# Global dependencies
list(APPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/cmake/modules/)

add_subdirectory(lib)
