SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11") 

# Live capture
add_executable (live-capture live-capture.cpp)
target_link_libraries (live-capture imageprocessors autotimer "-lopencv_core" "-lopencv_imgproc" "-lopencv_highgui" "-framework OpenCL")
