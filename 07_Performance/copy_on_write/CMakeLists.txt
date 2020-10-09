#
# CMakeLists.txt - cmake build file for API Design examples
#
# Martin Reddy, 1 Jan 2010 - http://APIBook.com/
#

# Declare the minimum version of cmake that we need
cmake_minimum_required(VERSION 2.4)

# Build the executable
add_executable(copy_on_write main.cpp)

# Set parent folder for organization in Visual Studio project
set_target_properties(copy_on_write PROPERTIES FOLDER "${VS_PARENT_FOLDER}")
