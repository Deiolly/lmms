INCLUDE(BuildPlugin)
INCLUDE_DIRECTORIES("${STK_INCLUDE_DIR}")
LINK_LIBRARIES(${STK_LIBRARY})
SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fexceptions")
BUILD_PLUGIN(malletsstk Mallets.cpp Mallets.h MOCFILES Mallets.h EMBEDDED_RESOURCES artwork.png logo.png)
