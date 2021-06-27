#Custom lib
set(Custom_LIB myLib)
#Bring the sources
file(GLOB SOURCES_LIB ${PROJECT_SOURCE_DIR}/src/lib/*.cpp)

#Generate library
add_library(${Custom_LIB} SHARED ${SOURCES_LIB})
#add_library(myLib STATIC ${SOURCES})

#Add other libraries used to build the main library
#target_link_libraries(myLib PRIVATE ${OpenCV_LIBS})

#Set an installation path, type "sudo make install" to apply
install(TARGETS ${Custom_LIB} DESTINATION /usr/lib)

