# DroneAidCameraModule

## Pre-requisites
- Raspbery Pi 3 or 4
- Raspberry Pi Camera
- Raspberry Pi Power Adapter
- Memory Card

## Installation

- Download Raspberry Pi Image:
https://www.raspberrypi.org/downloads/raspbian/
(Make sure to choose "Raspbian Buster with desktop and recommended software")
- Burn the image onto the SD Card with Etcher
https://www.balena.io/etcher/
- SSH into Raspberry Pi with terminal
- Enable Camera
```
pi@raspberry:~ $ sudo raspi-config
```
- Reboot Pi
```
sudo reboot
```
- Start server
```
python3 uav_live_stream.py
```
- Navigate to `http://localhost:8080` in browser
- To finish, shutdown the Raspberry Pi with the following command.
```
sudo shutdown -h now
```
*If Raspberry Pi is not shutdown correctly, it may cause memory loss and corruption.