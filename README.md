# slam14-final-project
Implement the stereo visual odometry, and evaluated in KITTI
## Install
The latest codes are tested on Ubuntu 16.04, OpenCV 3.4
## Data and Model
Download data in [KITTI's Visual Odometry Dataset (greyscale)](http://www.cvlibs.net/datasets/kitti/eval_odometry.php)
## Compile
```bash
mkdir build
cd build
cmake ..
make
```
## Run
After compilation, in the build directly  
```bash
./visual_odometry [sequence ID] [max frame] [optimize frame] [dataset directory]
```
