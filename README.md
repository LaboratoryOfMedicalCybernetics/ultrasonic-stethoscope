# Ultrasonic Stethoscope
Ultrasonic stethoscope is a device build on top of Arduino Due, PyQtgraph and NVidia CUDA. Device allows to get HQ sound (about 666 samples per second) and record ultrasonic range up to 333 kHz. Device is supposed to use for medical diagnostics of heart and lungs deseases.

This repo contains software for ultrasonic stethoscope and academic [paper](Paper) describing this project.

## Installation
1. Download and install [Anaconda](https://www.anaconda.com/download)
2. Install pyFFT and last version of pyserial (install it from conda forge channel)

## Running
Activate Anaconda environment and run app: `python app.py`(on windows just double-click `Stethoscope.bat`)

## Overview:
1. Input Signal
2. Ultrasonic mic
3. Amplifier
4. ADC (Arduino Due)
5. App: gets data from ADC,  plots hi-fps soundwawe in realtime, record data to file
6. App: send data to NVidia CUDA Server
7. CUDA Server: calculates fft very fast and sends fft.png (plot of signal's spectrum) back to client's app 

## Installation
1. download and install miniconda
2. Anaconda Prompt == conda root env
3. `install.bat` - он после gui установки miniconda активирует root enviroment, потом создает новую в текущей папке и 
4. активирует, все устанавливает
5. `stethoscope.bat` - активрирует и запускает 

## How this device looks:
<img src="docs/whitepaper/images/hardware.jpg" width=765px/>

## new installation
```sh
git clone https://github.com/tandav/ultrasonic-stethoscope.git
cd ultrasonic-stethoscope
python3 -m venv .steth
source .steth/bin/activate
pip install -r requirements.txt
python3 app.py # run
```
