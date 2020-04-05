# pre_config_pi

To pre configure your Raspberry Pi with your WIFI and enable VNC, SSH, GPIO, SERIAL we can do the following.

1. Download Rasbian Sketch from: https://www.raspberrypi.org/downloads/raspbian/
2. Mount the image to your SD card, using the command line or Etcher are two ways this can be done.
3. Once mouted, remove, then put the SD back into the machine
4. Open the root directory of the PI and you should see the operating system files
5. Open from within this repository, the wpa_supplicant.conf file
6. Add your WIFI credentials and save the file
7. Add the following files to the root of the SD card directory: vnc, ssh, gpio, serial, spa_supplicant.conf
8. Boot the PI.
9. Give it 5 minutes to boot the first time
10. Via your personal computer, in the terminal run - ssh pi@raspberrypi.local 
11. Type the password, raspberry
12. You now have access to the Pi, have fun!

Video walk through of these steps and a few more to get you up and running with your Raspberry Pi: 
https://www.youtube.com/watch?v=4p7navuQbh0&t=170s

For VNC Viewer - Run these command on the Pi via SSH before trying to connect to VNC Veiwer.

sudo apt update
sudo apt install realvnc-vnc-server realvnc-vnc-viewer

Some handy commands:

- Shut down the Pi - sudo shutdown -h now
- Enter Bios - sudo raspi-config
- List items in directory - ls
- Check IP - ifconfig
- Change Directory - cd
- Create file - touch foo.extension
- Create directory - mkdir bar
- Remove file - rm foo.extension
- Remove directory - rm -rf bar
- Move or Rename - mv foo.txt bar.txt
- Convert file type - convert foo.png bar.jpg



