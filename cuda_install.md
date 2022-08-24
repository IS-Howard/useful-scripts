## Steps:

```Shell
sudo apt install nvidia-driver-460
//version 460
```
reboot
```Shell
nvidia-smi  //check
```
```Shell
wget https://developer.download.nvidia.com/compute/cuda/11.2.1/local_installers/cuda_11.2.1_460.32.03_linux.run
//version 11.2.1
```
```Shell
sudo sh cuda_11.2.1_460.32.03_linux.run
```
```Shell
echo '# CUDA Soft Link' >> ~/.bashrc
echo 'export PATH=/usr/local/cuda-11.2/bin${PATH:+:${PATH}}' >> ~/.bashrc
echo 'export LD_LIBRARY_PATH=/usr/local/cuda-11.2/lib64${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}' >> ~/.bashrc
source ~/.bashrc
```
```Shell
nvcc -V //check 
```
install cudnn from website
```Shell
sudo cp ./cuda/include/cudnn.h /usr/local/cuda-11.2/include
sudo cp ./cuda/lib64/libcudnn* /usr/local/cuda-11.2/lib64
sudo chmod a+r /usr/local/cuda-11.2/include/cudnn.h /usr/local/cuda-11.2/lib64/libcudnn*
//version cudnn8.2.1.32
```
