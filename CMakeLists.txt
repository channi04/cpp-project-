cmake_minimum_required(VERSION 3.10)

include_directories(${OpenCV_INCLUDE_DIRS} C:/Users/cchan/Downloads/opencv/build/include/opencv2/core)


set(EXECUTABLE_DIR "C:/Users/cchan/Downloads/image-processing-algorithms-master/01-gradient/gradient.cpp")

project(image-processing-algorithms-master)

set(OpenCV_DIR C:/Users/cchan/Downloads/opencv/build)
find_package(OpenCV REQUIRED)

add_executable(${PROJECT_NAME} 01-gradient/gradient.cpp)

target_link_libraries(${PROJECT_NAME} ${OpenCV_LIBS})
