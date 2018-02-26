# movidius-work

# Installation Notes

Two important resource is used to install movidius SDK on Ubuntu 16.04


https://github.com/BVLC/caffe/wiki/Ubuntu-16.04-or-15.10-Installation-Guide

https://www.youtube.com/watch?v=fESFVNcQVVA

The basic steps followed after installing  git, etc. 

```
#caffe related dependencies
 sudo apt-get install libprotobuf-dev libleveldb-dev libsnappy-dev libopencv-dev libhdf5-serial-dev protobuf-compiler
 sudo apt-get install --no-install-recommends libboost-all-dev
 sudo apt-get install libgflags-dev libgoogle-glog-dev liblmdb-dev
 sudo apt-get install libatlas-base-dev
 
#if you have a anaconda installed you should update the protobuf
 conda install protobuf
 
#python related dependencies , this for both py27 and py3
 sudo apt-get install -y python-pip
 sudo apt-get install -y python-pip3
 sudo apt-get install -y python-dev
 sudo apt-get install -y python-numpy python-scipy
 sudo apt-get install -y python3-dev
 sudo apt-get install -y python3-numpy python3-scipy

```

after the steps above you can start the movidies install
```
git clone http://github.com/Movidius/ncsdk
cd ncsdk
make install
make examples
```

