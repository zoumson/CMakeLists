cmake_minimum_required(VERSION 2.8.9)

#set the project name
project (serie2)

#Set the compiler
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_BUILD_TYPE Release)
set( LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)

#Set ccache (for speeding up)
find_program(CCACHE_FOUND ccache) 
if(CCACHE_FOUND) 
    set_property(GLOBAL PROPERTY RULE_LAUNCH_COMPILE ccache) 
    set_property(GLOBAL PROPERTY RULE_LAUNCH_LINK ccache) 
endif(CCACHE_FOUND) 
set (CMAKE_CXX_FLAGS "-DPCL_ONLY_CORE_POINT_TYPES=ON -DNO_EXPLICIT_INSTANTIATIONS") 

############### Dependencies #######################

#Add opencv cmake .config path
#set (OpenCV_DIR opt/opencv/release)

#Find opencv libs
#ind_package(OpenCV 4.5.1 REQUIRED)

############### My Files #########################

#Bring the headers
include_directories(${PROJECT_SOURCE_DIR}/include)

#Bring the library
#Custom lib
set(Custom_LIB myLib)
#Bring the sources
file(GLOB SOURCES_LIB ${PROJECT_SOURCE_DIR}/src/*.cpp)

#Generate library
add_library(${Custom_LIB} SHARED ${SOURCES_LIB})
#add_library(myLib STATIC ${SOURCES})

#Add other libraries used to build the main library
#target_link_libraries(myLib PRIVATE ${OpenCV_LIBS})

#Set an installation path, type "sudo make install" to apply
install(TARGETS ${Custom_LIB} DESTINATION /usr/lib)





