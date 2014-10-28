cmake_minimum_required(VERSION 2.8.4)
project(CardGame)

#set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

find_package ( SDL REQUIRED )

set(SOURCE_FILES main.cpp)
add_executable(CardGame ${SOURCE_FILES})
target_link_libraries( CardGame ${SDL_LIBS} )