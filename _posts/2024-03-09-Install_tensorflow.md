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

1. Install Visual Studio Community 2015-2019 

TensorFlow in Native Windows requires Microsoft Visual C++ Redistributable for [Visual Studio 2015, 2017, and 2019](https://download.visualstudio.microsoft.com/download/pr/4100b84d-1b4d-487d-9f89-1354a7138c8f/5B0CBB977F2F5253B1EBE5C9D30EDBDA35DBD68FB70DE7AF5FAAC6423DB575B5/VC_redist.x64.exe) (Do not install the lastest version, e.g., 2022)


2. Install NVIDIA graphics drivers  

> Before going further, make sure that your NVIDIA Graphic card is supported Machine learning/Deep learning capability with **compute capability of higher equal 3.0** <https://developer.nvidia.com/cuda-gpus>  

If your graphic card is suitable for ML/DL with a suitable compute capability, you can download and install the latest version of the graphic card driver by selecting your corresponding card's specs. Then, you can install the driver by applying default options.  

![Download NVIDIA graphic driver](/assets/images/2024/2024-03-10-image_01.jpg)  


3. Install CUDA resources  

 - Download and install [CUDA Toolkit 11.8](https://developer.nvidia.com/cuda-11-8-0-download-archive?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exe_local)   

![Cuda Toolkit 11.8](/assets/images/2024/2024-03-10-image_02.jpg)  
 
- Download [cuDNN SDK 8.6.0 (for CUDA 11.x for Windows)](https://developer.nvidia.com/rdp/cudnn-archive). You then need to extract the cuDNN files, copy and paste all files and folders into the CUDA install location. E.g., *C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.8*   

Open the **Environmental Variables** and add two new paths:
```
C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.8\bin   
C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.8\libnvvp 
```

4. Install Anaconda 3  

- Download and install [Anaconda 3](https://www.anaconda.com/download#downloads)  

Then, open **Environment variable** and add three more paths (under PATH)   
> C:\Users\yourusername\anaconda3   
> C:\Users\yourusername\anaconda3\Library\bin   
> C:\Users\yourusername\anaconda3\Scripts   

- Create a new virtual environment 





https://www.lavivienpost.com/install-tensorflow-gpu-on-windows-complete-guide/ 

### Fix kernel dies when running tensorflow code

https://github.com/microsoft/vscode-jupyter/issues/9157

