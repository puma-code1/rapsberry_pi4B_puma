cmake_minimum_required(VERSION 3.2)

project(gpio)
set(CMAKE_BUILD_TYPE Debug)

set(CMAKE_INSTALL_PREFIX ${PROJECT_SOURCE_DIR})

set(DIVISIBLE_INSTALL_INCLUDE_DIR ${PROJECT_SOURCE_DIR}/inc)
set(DIVISIBLE_INSTALL_BIN_DIR ${PROJECT_SOURCE_DIR}/bin)
set(DIVISIBLE_INSTALL_LIB_DIR ${PROJECT_SOURCE_DIR}/lib)


set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)



file(GLOB SRC_FILES ${PROJECT_SOURCE_DIR}/src/*.cpp)

include_directories(${DIVISIBLE_INSTALL_INCLUDE_DIR})

add_executable( gpio ${SRC_FILES})

#add_subdirectory(src)

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          