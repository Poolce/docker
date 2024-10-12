FROM ubuntu:22.04
WORKDIR /home
RUN apt-get update
RUN apt-get install -y wget


RUN wget https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/cuda-keyring_1.1-1_all.deb
RUN dpkg -i cuda-keyring_1.1-1_all.deb
RUN apt-get update
RUN apt-get -y install cuda-toolkit-12-6
RUN export LD_LIBRARY_PATH=/usr/local/cuda-12.6/lib64:$LD_LIBRARY_PATH
RUN export PATH=/usr/local/cuda-12.6/bin:$PATH
