# Vision

## Goals for vision this year

This year, our goal was to use vision in conjunction with odometery readings to get an accurate Pose (or location of the robot on the field) even after being battered by other robots, which if odometry was left on its own, would have led to a more and more inaccurate Pose.

## Installing PhotonVision and Photonlib

In contrast to last years Limelight 2, we chose the Orange Pi as our coprocessor of choice. Here is a general guide for the orange pi with photonvision: [Orange Pi Docs](https://docs.google.com/document/d/1DAPOnU2NfOp91UnMQnkhyiUAanlCDJ6zl_YsCkCMZdA/edit) Keep in mind, the docs are just notes that someone made while they were trying out the Orange Pi and all the info there should be taken with a grain of salt. We bought two Orange Pi 5's. On a microSD card, we flashed the image for the pi, which can be found here. [Latest Releases](https://github.com/PhotonVision/photonvision/releases). Make sure to download the img that is meant for the Orange Pi 5, not the 5 Plus. We used Balena Etcher to flash the image on the card. Put the SD card into the Pi. 
>**Please use caution to not pop out the sd card or unplug the Pi while the Pi is on. If you do manage to screw up and do this please refer to: [What to do if I popped out the SD card](#what-to-do-if-i-popped-out-the-sd-card)**
>
After the pi boots up, the login is "pi" and the password is "raspberry". 

## What to do if I popped out the SD card

If you popped out your SD card or unplugged the Pi while it had power, then you did not follow my directions. You most likley lost all the calibrations and settings you had on the SD card because its now corrupted. You need to re-flash your 