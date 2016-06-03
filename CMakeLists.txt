PROJECT( SolarEngine)

CMAKE_MINIMUM_REQUIRED( VERSION 2.8 )

option(SOLAR_BUILD_WITH_UNICODE "Build with unicode(wide-byte) or ansi(multi-byte)." TRUE)

SET_PROPERTY(GLOBAL PROPERTY USE_FOLDERS ON)
set( SALVIA_HOME_DIR ${CMAKE_HOME_DIRECTORY} )

# Configuring
#include (${CMAKE_HOME_DIRECTORY}/cmake/SystemInfo.cmake)
#include (${CMAKE_HOME_DIRECTORY}/cmake/ConfigCompiler.cmake)
#include (${CMAKE_HOME_DIRECTORY}/cmake/Variables.cmake)
#include (${CMAKE_HOME_DIRECTORY}/cmake/ConfigurePath.cmake)
#include (${CMAKE_HOME_DIRECTORY}/cmake/ConfigBoostLibs.cmake)
#include (${CMAKE_HOME_DIRECTORY}/cmake/ConfigLLVMLibs.cmake)
ADD_SUBDIRECTORY( cmake )

# Add projects
ADD_SUBDIRECTORY( solar)



