#
# CMakeLists.txt - cmake build file for API Design examples
#
# Martin Reddy, 1 Jan 2010 - http://APIBook.com/
#

# Declare the minimum version of cmake that we need
cmake_minimum_required(VERSION 2.4)

# create the libraries
add_executable(factory_extensible main.cpp rendererfactory.cpp)

# Set parent folder for organization in Visual Studio project
set_target_properties(factory_extensible PROPERTIES FOLDER "${VS_PARENT_FOLDER}")
