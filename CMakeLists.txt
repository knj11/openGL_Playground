cmake_minimum_required( VERSION 3.20 )

project( openGL_Playground )

set( GLFW_BUILD_DOCS OFF CACHE BOOL  "GLFW lib only" )
set( GLFW_INSTALL OFF CACHE BOOL  "GLFW lib only" )

add_subdirectory( glfw )

# include_directories("${GLFW_SOURCE_DIR}/deps")
# set( GLAD_GL "${GLFW_SOURCE_DIR}/deps/glad/gl.h" )
include_directories( include )

SET( CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} /ENTRY:mainCRTStartup" )

set( openGL_Playground-SRC
        src/main.cpp
        src/glad.c
        src/stb_image.cpp
)

add_executable( openGL_Playground ${openGL_Playground-SRC} )

target_link_libraries( openGL_Playground glfw )