cmake_minimum_required(VERSION 3.10.2)

project( K_MEANS)

find_package( ITK REQUIRED )
include( ${ITK_USE_FILE} )

add_executable( kMeans K_MEANS.cpp )
target_link_libraries( kMeans ${ITK_LIBRARIES} )