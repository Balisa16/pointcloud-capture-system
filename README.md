# D455-Sampling
Sampling code for D455 Camera

## Dependencies
### GLFW3
```
sudo apt install libglfw3-dev
```
or
```
sudo apt install libxrandr-dev libxinerama-dev libxcursor-dev libxi-dev -y
git clone https://github.com/glfw/glfw.git
cd glfw && mkdir build && cd build
cmake ..
make -j4
sudo make install
```
### Eigen3
```
sudo apt install libeigen3-dev -y
```
### GLEW
```
sudo apt-get install -y libglew-dev
```
### Pangolin
```
https://github.com/stevenlovegrove/Pangolin.git
cd Pangolin
mkdir build && cd build
cmake ..
make -j4
sudo make install
```
or use
```
sudo apt-get install libpango-1.0-0
```
\
Please recheck your pangolin installation with
```
echo $LD_LIBRARY_PATH
```
if in these path there is no ```libpango_core.so```, add it with 
```
export LD_LIBRARY_PATH=/path/to/directory:$LD_LIBRARY_PATH
```
in *~/.bashrc* and update ```source ~/.bashrc```. ***/path/to/directory*** is path of directory which contains libpango_core.so. Usually in */usr/local/lib*
