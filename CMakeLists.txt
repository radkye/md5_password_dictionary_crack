cmake_minimum_required(VERSION 3.0)

# Name the application
SET( PROJ_NAME      "md5" )

project( $(PROJ_NAME) )

# Compiler Settings
add_definitions( -std=c++14 -Wextra -Wall -O2 )

# Enable Tests for CMake
include(CTest)

add_subdirectory( src )
add_subdirectory( test )
