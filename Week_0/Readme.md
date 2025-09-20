# System Information and Tool Installation Guide

#### This guide provides instructions to install the essential EDA tools required for the RISC-V Chip Tapeout project.
---

## System Information

<p align="center">
  <img src="https://github.com/user-attachments/assets/485a9f01-ade5-4b12-973c-f93bded882f6" 
       alt="Screenshot from 2025-09-20 21-26-29" 
       width="563" 
       height="266"/>
</p>

---

## Tool Installation 

### 1. Yosys 

``` bash
git clone https://github.com/YosysHQ/yosys.git
cd yosys
git submodule update --init --recursive
sudo apt-get install build-essential clang lld bison flex libfl-dev \
	libreadline-dev gawk tcl-dev libffi-dev git \
	graphviz xdot pkg-config python3 libboost-system-dev \
	libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc
make
sudo make install
```

### 2. Iverilog

``` bash
sudo apt-get update
sudo apt-get install iverilog
```

### 3. GTKWave

``` bash
sudo apt-get update
sudo apt-get install gtkwave
```

### 4. Ngspice

``` bash
sudo apt-get update
sudo apt-get install ngspice
```

### 5. Magic VLSI Layout Tool

``` bash
sudo apt-get install m4
sudo apt-get install tcsh
sudo apt-get install csh
sudo apt-get install libx11-dev
sudo apt-get install tcl-dev tk-dev
sudo apt-get install libcairo2-dev
sudo apt-get install mesa-common-dev libglu1-mesa-dev
sudo apt-get install libncurses-dev

git clone https://github.com/RTimothyEdwards/magic
cd magic

./configure

make

sudo make install
```
---

## Tool Verification

### 1. Yosys 
<p align="center">
  <img src="Week_0/img/yosys_setup.png" alt="Description of image" width="600"/>
</p>

### 2. Iverilog

<p align="center">
  <img src="Week_0/img/iverilog_setup.png" alt="Description of image" width="600"/>
</p>

### 3. GTKWave

<p align="center">
  <img src="Week_0/img/gtkwave_setup.png" alt="Description of image" width="600"/>
</p>

### 4. Ngspice
<p align="center">
  <img src="Week_0/img/ngspice_setup.png" alt="Description of image" width="600"/>
</p>

### 5. Magic VLSI Layout Tool
<p align="center">
  <img src="Week_0/img/magic_setup.png" alt="Description of image" width="600"/>
</p>
