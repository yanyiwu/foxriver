SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)
SET(LIBRARY_OUTPUT_PATH ${PROJECT_BINARY_DIR}/lib)

INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR} ${PROJECT_SOURCE_DIR}/src ${PROJECT_SOURCE_DIR}/src/CppJieba)
ADD_DEFINITIONS(-std=c++0x -O3 -Wall -g)

ADD_EXECUTABLE(foxriver main.cpp)
TARGET_LINK_LIBRARIES(foxriver tinyxml2 pthread)
