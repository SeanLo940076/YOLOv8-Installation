# YOLOv8-Installation
 YOLOv8 Installation Guide

## Introduction
This guide provides detailed instructions for installing YOLOv8 on Ubuntu systems, including the installation of TensorFlow, PyTorch, and other necessary Python packages.


## Installation Steps

## Update System and Install pip
```bash
sudo apt update
sudo apt install -y python3-pip
pip3 install --upgrade pip
```

## Installation Tensorflow
```bash
pip3 install tensorflow
or
pip3 install --user --upgrade tensorflow
```

## Verify Installation

```bash
python3 -c "import tensorflow as tf; print(tf.reduce_sum(tf.random.normal([1000, 1000])))"
```


## Installation Pytorch

```bash
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

## Installation YOLOv8
```bash
cd ~/Documents
git clone git@github.com:ultralytics/ultralytics.git
cd ultralytics
gedit requirements.txt
	opencv --> correspond opencv version

pip3 install python-dateutil --upgrade
sudo apt-get -y install libcanberra-gtk-module
pip3 install -r requirements.txt 
pip3 install ultralytics
```