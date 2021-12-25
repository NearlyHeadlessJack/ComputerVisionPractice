project(Camera_Calibration)
set(CMAKE_CXX_STANDARD 11)

find_package(OpenCV 4.5.4 QUIET)
if(NOT OpenCV_FOUND)    
    find_package(OpenCV 2.4.3 QUIET)
    if(NOT OpenCV_FOUND)
        message(FATAL_ERROR "OpenCV > 2.4.3 not found.")
    endif()
endif()

include_directories(${OpenCV_INCLUDE_DIR})
add_executable(Camera_Calibration camera_calibration.cpp)
target_link_libraries(Camera_Calibration ${OpenCV_LIBS})
