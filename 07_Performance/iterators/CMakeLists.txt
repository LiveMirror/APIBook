#
# CMakeLists.txt - cmake build file for API Design examples
#
# Martin Reddy, 1 Jan 2010 - http://APIBook.com/
#

# Declare the minimum version of cmake that we need
cmake_minimum_required(VERSION 2.4)

# Define the include/link directories
include_directories("${CMAKE_CURRENT_SOURCE_DIR}/../auto_timer")
link_directories("${CMAKE_CURRENT_BINARY_DIR}/../auto_timer")

# Build the executable
add_executable(iterators main.cpp value.cpp)

# Link against the AutoTimer library
target_link_libraries(iterators autotimer)

# Set parent folder for organization in Visual Studio project
set_target_properties(iterators PROPERTIES FOLDER "${VS_PARENT_FOLDER}")
