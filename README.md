# Horus: An Interactive Tool for Designing Quadrotor Camera Shots

Homepage: http://stanford-gfx.github.io/Horus/

This repository provides the source code for the tool presented in our SIGGRAPH Asia 2015 paper.

## Usage Instructions

Horus is an in-browser Javascript application with a custom Python backend. It relies on the Google Earth NSAPI plugin and Google Chromium. It has been exclusively tested on Mac OS X. Note that this is a research prototype, and contains experimental and untested code. It is released here to aid researchers in reproducing our results.

https://docs.google.com/document/d/1t-euYONWhzXfZr2kS9Qt8z9R9N8hgF3YIWdFDxR72AI/edit

### Running on Ubuntu 14.04

Notice:
* This won't work with Docker, too much compilation involved, and even vm with 4gb of rams can't hold it.
* Works with Vagrant, used [this image](https://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box)
* Pip commands bellow should be executed separately or else will fail

```
apt-get update
apt-get install -y python-dev python-pip pkg-config libpng3 libfreetype6 libfreetype6-dev libjpeg-dev  libblas-dev liblapack-dev gfortran
pip install numpy cython scipy
pip install pandas
pip install pylab flask flask-restful cvxopt pymavlink
cd /vagrant/horus/Code/HorusApp
python run.py
```
