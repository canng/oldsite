---
title: Set-up Windows 10 machine for Deep Learning
layout: post
image: assets/images/2024/2024-03-10-tensorflow_windows.jpg
categories:
- post
- python
tags:
- python
- tips
featured: false
hidden: false
comments: false
---

## Install TensorFlow GPU on Windows 10 (NVIDIA graphic card)

> 
> My PC specs:   
> MSI GF 63 8RD    
> Intel Core i5 8300H CPU @2.30GHz (4 Cores, 8 Threads)   
> RAM 24 GB (upgraded)   
> Graphics: NVIDIA GeForce GTX 1050 Ti with Max-Q and Intel(R) UHD Graphics 630   
> 

1. Install NVIDIA graphics drivers

> Before going further, make sure that your NVIDIA Graphic card is supported Machine learning/Deep learning capability with **compute capability of higher equal 3.0** <https://developer.nvidia.com/cuda-gpus>

If your graphic card is suitable for ML/DL with a suitable compute capability, you can download and install the latest version of the graphic card driver by selecting your corresponding card's specs. Then, you can install the driver by applying default options.

[!Download NVIDIA graphic driver!](/assets/images/2024/2024-03-10-image_01.jpg)


2. Install CUDA resources

 - Download and install [CUDA Toolkit 11.8](https://developer.nvidia.com/cuda-11-8-0-download-archive?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exe_local)   

[!Cuda Toolkit 11.8!](/assets/images/2024/2024-03-10-image_02.jpg)
 
- 

https://www.lavivienpost.com/install-tensorflow-gpu-on-windows-complete-guide/ 

### Fix kernel dies when running tensorflow code

https://github.com/microsoft/vscode-jupyter/issues/9157

