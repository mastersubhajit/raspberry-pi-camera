# Video Streaming with Raspberry Pi Camera Module
<p align="center">
  <img alt="PICTURE logo" src="https://github.com/mastersubhajit/mastersubhajit.github.io/blob/ea26211930efe2811005977d43f106c960af6d79/pi-cam.png" width="400">
  <br>
  <b>Video streaming with a Raspberry Pi and a Pi Camera module to stream live footage from a webpage that you can access in any device that has a browser and is connected to the same network.</b>
  <br>
  <br>
</p>

## Compatibility and Tested Raspberry Pi Versions: 

| Model | Compatible | Tested |
| ------- | --------- | --------- |
| Raspberry Pi Pico | ❌ | ✅ |
| Raspberry Pi Zero WH | ✅ | ✅ |
| Raspberry Pi Zero W | ✅ | ✅ |
| Raspberry Pi Zero 2W | ✅ | ❌ |
| Raspberry Pi Zero | ✅ | ✅ |
| Raspberry Pi 2 | ✅ | ❌ |
| Raspberry Pi 3 / 3B+ | ✅ | ❌ |
| Raspberry Pi 4 | ✅ | ✅ |
| Raspberry Pi 400 | ✅ | ❌ |

## Installation

If you’re using the Raspberry Pi Camera Module, you need to enable the camera software in your Raspberry Pi in order to use it. In the Desktop environment, go to the Raspberry Pi Configuration window under the Preferences menu, open the Interfaces tab and enable the Camera as shown in figure below:
<p align="center">
  <img alt="PICTURE" src="https://github.com/mastersubhajit/mastersubhajit.github.io/blob/8150d5f8efc7892f3bc51936ea73588285a60559/assets/images/Desktop_interface_rpi_camera.webp" width="500">
</p>

 Or, in the Terminal window, type the following command:
`pi@raspberry:~ $ sudo raspi-config`

You should see the Raspberry Pi software configuration tool: 
Select the Interfacing Options -> Enable the camera and reboot.

## Find the Pi's IP address

To access your video streaming web server, you need to know your Raspberry Pi IP address. For that, use the following command:
`pi@raspberry:~ $ ifconfig`

You’ll be given a bunch of information, including your Raspberry Pi IP address for example: `192.168.x.xxx`

## Download the Script from this Repository

`git clone https://github.com/mastersubhajit/video_streaming_with_raspberry_pi_camera_module.git`

## Accessing the Live Stream

First run the script:
`pi@raspberrypi:~ $ python3 raspberry_pi_camera_streaming.py`

Once the script is running, you can access your video streaming web server at: `<Your_Pi_IP_Address>:8000`

You can access the video streaming through any device that has a browser and is connected to the same network that your Pi.
