cmake_minimum_required(VERSION 2.8)

project(cmake-findpthreads)
set(CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")
find_package( Pthreads )

message(STATUS "Pthreads found: ${Pthreads_FOUND}")
message(STATUS "Pthreads includes: ${Pthreads_INCLUDE_DIRS}")
message(STATUS "Pthreads libraries: ${Pthreads_LIBRARIES}")
message(STATUS "Pthreads version: ${Pthreads_VERSION_STRING}")
