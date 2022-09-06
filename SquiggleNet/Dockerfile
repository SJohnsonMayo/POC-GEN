##FROM --platform=linux/arm64 pytorch/pytorch:1.10.0-cuda11.3-cudnn8-runtime
##FROM armswdev/pytorch-arm-neoverse:r22.06-torch-1.11.0-onednn-acl

FROM python:3.9


RUN apt-get -y update
RUN apt-get install -y libz-dev wget git build-essential python3-pip git

##RUN sudo apt-get update && apt-get install -y python3 python3-pip git

RUN pip3 install scipy numpy click ont-fast5-api torch

RUN git clone https://github.com/welch-lab/SquiggleNet
