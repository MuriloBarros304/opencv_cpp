cmake_minimum_required(VERSION 3.10)

project(DetectCircles)

set(OpenCV_DIR /home/murilo/opencv/build)
find_package(OpenCV REQUIRED)

add_executable(${PROJECT_NAME} detectcirc.cpp main.cpp)

target_link_libraries(${PROJECT_NAME} ${OpenCV_LIBS})