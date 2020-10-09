#
# CMakeLists.txt - cmake build file for API Design examples
#
# Martin Reddy, 1 Jan 2010 - http://APIBook.com/
#

# Declare the minimum version of cmake that we need
cmake_minimum_required(VERSION 2.4)

# Build the executable
add_executable(stack_datadriven main.cpp stack.cpp arglist.cpp)

# Build the test program for the arglist module
add_executable(arglist_test arglist_test.cpp arglist.cpp)

# Set parent folder for organization in Visual Studio project
set_target_properties(stack_datadriven PROPERTIES FOLDER "${VS_PARENT_FOLDER}")
set_target_properties(arglist_test PROPERTIES FOLDER "${VS_PARENT_FOLDER}")
