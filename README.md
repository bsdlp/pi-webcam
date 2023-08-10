# Raspberry Pi Webcam

## Use cases

* [Remote OBS media source](https://obsproject.com/wiki/Sources-Guide#media-source)

## Usage

1. Install raspbian buster lite

2. Boot up your raspberry pi and make sure it is reachable on the network.

3. Ensure ansible is installed on your computer

4. Clone this repo somewhere onto your computer

5. Edit the `inventory` file, replacing `benchcam-1.catnet` with your pi's network address, and the `ansible_user` value to the user you use to ssh into your pi.

6. In this repo's working directory, run `ansible-playbook main.yml`.

After your pi reboots, you can access the UV4L web frontend at `https://<your pi's network address>:8080`. You can find the video stream in the MJPEG/stills stream link.

## Sources

* https://www.linux-projects.org/uv4l/installation/
* https://www.linux-projects.org/documentation/uv4l-raspicam/
* http://www.davidhunt.ie/raspberry-pi-high-quality-camera-setup-for-low-latency-video-conferencing/
* https://www.raspberrypi.com/documentation/computers/configuration.html#list-of-options26
* https://codecalamity.com/raspberry-pi-hardware-encoding-speed-test/
