#
# CMakeLists.txt - cmake build file for API Design examples
#
# Martin Reddy, 1 Jan 2010 - http://APIBook.com/
#

# Declare the minimum version of cmake that we need
cmake_minimum_required(VERSION 2.4)

# Shared variables for all child CMakeLists.txt
set(VS_PARENT_FOLDER "08_Versioning")

# Specify the subdirectories to build
add_subdirectory(version_api)
add_subdirectory(deprecate_compiletime)
add_subdirectory(deprecate_runtime)
