cmake_minimum_required(VERSION 3.0)

project(PJG)

find_package(SDL2 REQUIRED)
find_package(SDL2_image REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS} ${SDL2_IMAGE_INCLUDE_DIRS})

add_executable(PJG src/main.cpp)

target_link_libraries(PJG ${SDL2_LIBRARIES} ${SDL2_IMAGE_LIBRARIES})