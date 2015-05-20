cmake_minimum_required(VERSION 2.8)
SET( CMAKE_CXX_FLAGS  "${CMAKE_CXX_FLAGS} -g" )
project( Neuonas )
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable( Neuronas Estabilizador.cpp )
target_link_libraries( Neuronas ${OpenCV_LIBS} )

