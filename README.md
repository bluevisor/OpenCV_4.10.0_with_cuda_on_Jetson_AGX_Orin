Setup Nvidia Jetson AGX Orin:

1, Install Jetpack 6 using NVIDIA's SDK Manager, from an X86 Ubuntu 20.04 via USB (hold Recovery and Reset for 2 seconds)

2, Change Power mode to MAXN

3, Install Chromeium via Ubuntu Software app

4, Install jtop: `sudo apt update`, `sudo apt install python3-pip`, `sudo pip3 install jetson-stats`

5, Install OpenCV with Cuda: download the shell script from this repo, `chmod +x install_OpenCV_4.10.0_with_cuda_on_Jetpack_6.sh`, `sudo ./install_OpenCV_4.10.0_with_cuda_on_Jetpack_6.sh`

6, Install missing Cuda and TensorRT: `sudo apt-get install tensorrt nvidia-tensorrt-dev python3-libnvinfer-dev`

p.s. *Do not use U.S. apt mirror
