#Custom lib
set(Custom_LIB myLib)
#Bring the sources
file(GLOB SOURCES_DEMO ${PROJECT_SOURCE_DIR}/src/demo/*.cpp)

#Build the executable
add_executable(demo ${SOURCES_DEMO})

#Link the libraries 
target_link_libraries(demo ${Custom_LIB})

