# CUDA-installation-on-Centos-6.10
I'd like to share my experience of CUDA installation on Centos 6.10

I've tried several times to install CUDA on my machine in which Centos 6.10 and NVIDIA TITAN X maxwell (GM200 GPU) are installed.
In this installation it is very important to match the version of graphic driver, gcc compiler, kernel version and CUDA software simultaneously.

In my case I decided to use Centos 6 which means gcc compiler version and kernel version are fixed. So I had to find a proper version of graphic driver for TITAN X. If I find then I looked at the CUDA version. This is one of the ways you can choose.
You can fix graphic card first, then you can find OS and CUDA version.

I will summarize these things as a table shortly not this time...

NVIDIA has provided the unix version driver for TITAN X maxwell since the version 349.77 so I started off with the oldest one but it couldn't generate linux kernel properly on Centos 6.10. 
My next shot was on 375.66 and it worked. 
So my environment is as follows: Centos 6.10, Graphic Driver 375.66, Cuda 8.0
