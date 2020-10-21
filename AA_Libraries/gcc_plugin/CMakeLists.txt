#
# CMakeLists.txt - cmake build file for API Design examples
#
# Martin Reddy, 1 Jan 2010 - http://APIBook.com/
#

# Declare the minimum version of cmake that we need
cmake_minimum_required(VERSION 2.4)

# create the library
add_library(plugin SHARED plugin.cpp)
set_target_properties(plugin PROPERTIES FOLDER "${VS_PARENT_FOLDER}")

add_executable(gcc_plugin main.cpp)
find_library(DL_LIB dl)
target_link_libraries(gcc_plugin ${DL_LIB})

# Set parent folder for organization in Visual Studio project
set_target_properties(gcc_plugin PROPERTIES FOLDER "${VS_PARENT_FOLDER}")
