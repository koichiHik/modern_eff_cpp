cmake_minimum_required(VERSION 3.0.0)
project(modern_eff_cpp VERSION 0.1.0)

include(CTest)
enable_testing()

#find_package(Boost REQUIRED)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_CXX_FLAGS 
  ${CMAKE_CXX_FLAGS} "-Wall -std=c++14")

#set(CMAKE_CXX_FLAGS 
#  ${CMAKE_CXX_FLAGS} "-O0 -Weffc++ -Wall -Wextra -pedantic -Wconversion -Wdouble-promotion")

add_subdirectory(src/chap_1)
add_subdirectory(src/chap_2)
add_subdirectory(src/chap_3)
add_subdirectory(src/chap_4)
add_subdirectory(src/chap_5)
add_subdirectory(src/chap_6)
add_subdirectory(src/chap_7)
add_subdirectory(src/chap_8)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)

