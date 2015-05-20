cmake_minimum_required(VERSION 2.8)
SET( CMAKE_CXX_FLAGS  "${CMAKE_CXX_FLAGS} -g" )
project( Codigo )
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable( Codigo Estabilizador.cpp )
target_link_libraries( Codigo ${OpenCV_LIBS} )

