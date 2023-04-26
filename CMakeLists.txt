cmake_minimum_required(VERSION 3.25 FATAL_ERROR)

project(yxwminiSTL
    VERSION         0.0.1
    DESCRIPTION     "yxwwindows's CMake miniSTL"
    HOMEPAGE_URL    "https://github.com/learningintheworld/yxwminiSTL"
    LANGUAGES       C CXX
)

list(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")
include(BuildInfo)

add_subdirectory(external)

add_subdirectory(src)

add_subdirectory(docs)

add_subdirectory(text)

add_subdirectory(packaging)