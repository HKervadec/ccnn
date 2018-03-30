project( ccnn )
cmake_minimum_required(VERSION 2.8)
add_definitions( -DLBFGS_FLOAT=32 )
set( CMAKE_POSITION_INDEPENDENT_CODE True )

find_package( PythonInterp 3.6 REQUIRED )
find_package( PythonLibs 3 REQUIRED )

list(APPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/cmake )
add_subdirectory( lib )