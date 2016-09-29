cmake_minimum_required(VERSION 3.3)

project(boost_mpl)

add_library(boost_mpl INTERFACE)

target_include_directories(boost_mpl BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_mpl DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
