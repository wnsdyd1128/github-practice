cmake_minimum_required(VERSION 3.5)
project(INHA_OSAP_001_FROYO)

# Default to C99
if(NOT CMAKE_C_STANDARD)
  set(CMAKE_C_STANDARD 99)
endif()

# Default to C++14
if(NOT CMAKE_CXX_STANDARD)
  set(CMAKE_CXX_STANDARD 14)
endif()

add_executable(set set_main.cc src/avltree.cc src/bst.cc src/set.cc)
target_include_directories(set PRIVATE ./include ./src)