FROM python:3.9

RUN apt-get -y update
RUN apt-get install -y python3-venv libz-dev wget git build-essential python3-pip

RUN apt-get install -y software-properties-common
RUN apt-get -y update
RUN apt-get install -y libhdf5-serial-dev

RUN git clone --recursive https://github.com/SJohnsonMayo/UNCALLED.git
RUN cd UNCALLED && python3 setup.py build_ext --library-dirs /usr/lib/aarch64-linux-gnu/hdf5/serial/lib/ --include-dirs /usr/lib/aarch64-linux-gnu/hdf5/serial/include/

RUN pip install --upgrade numpy==1.17.4
RUN cd UNCALLED && python3 setup.py install --user
## RUN apt install numpy


