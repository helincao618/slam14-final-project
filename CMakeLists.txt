CMAKE_MINIMUM_REQUIRED( VERSION 2.8 )

PROJECT( visual_odometry )
SET( CMAKE_CXX_FLAGS "-std=c++11")

find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS})

file(
    "src/visual_odometry.h"
    "src/visual_odometry.cpp"
)
add_executable( visual_odometry ${visual_odometry} )
target_link_libraries( visual_odometry
    ${OpenCV_LIBS}
)
