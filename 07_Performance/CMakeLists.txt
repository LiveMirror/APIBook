#
# CMakeLists.txt - cmake build file for API Design examples
#
# Martin Reddy, 1 Jan 2010 - http://APIBook.com/
#

# Declare the minimum version of cmake that we need
cmake_minimum_required(VERSION 2.4)

# Shared variables for all child CMakeLists.txt
set(VS_PARENT_FOLDER "07_Performance")

# Specify the subdirectories to build
add_subdirectory(auto_timer)
add_subdirectory(const_reference)
add_subdirectory(getter_speed)
add_subdirectory(virtual_speed)
add_subdirectory(struct_size)
add_subdirectory(copy_on_write)
add_subdirectory(iterators)
