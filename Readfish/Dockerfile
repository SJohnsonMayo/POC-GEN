# Set the base image to Ubuntu 18.04 and NVIDIA GPU
FROM --platform=linux/arm64 nvidia/cuda:11.1.1-base-ubuntu18.04



RUN apt-get -y update
RUN apt-get install -y python3.7 python3.7-dev python3.7-venv python3-venv libz-dev wget git build-essential python3-pip

RUN pip3 install --upgrade pip

RUN pip install git+https://github.com/LooseLab/read_until_api_v2@master
RUN pip install git+https://github.com/LooseLab/readfish@master

