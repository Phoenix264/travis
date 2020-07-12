cmake_minimum_required(VERSION 3.5)

project(travis_prj LANGUAGES CXX VERSION 0.0.1)

find_package(Boost COMPONENTS unit_test_framework REQUIRED)

configure_file(version.h.in ${PROJECT_SOURCE_DIR}/version.h)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(travis_prj main.cpp)
