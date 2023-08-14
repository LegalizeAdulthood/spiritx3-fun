cmake_minimum_required(VERSION 3.22 FATAL_ERROR)

project(spiritx3-fun)

include(CTest)

set_property(GLOBAL PROPERTY USE_FOLDERS ON)

set(Boost_NO_WARN_NEW_VERSIONS 1)
find_package(Boost REQUIRED COMPONENTS filesystem)

add_subdirectory(src)
if(BUILD_TESTING)
    add_subdirectory(test)
endif()
