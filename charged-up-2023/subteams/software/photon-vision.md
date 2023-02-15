# PhotonVision

## What is PhotonVision

The goal of PhotonVision is to get the limelight to sense the AprilTags. PhotonVision is the only compatible software we found online that works with FRC. PhotonVision is essenstially OS that runs on the limelight. For more information visit their main website: [PhotonVision Main Site](https://docs.photonvision.org/en/latest/)

## How to Set Up PhotonVision

## Download PhotonVision

[Download Steps](https://www.balena.io/etcher/)

For the limelight, head on over to the [PhotonVision Gitub Page](https://github.com/photonvision/photonvision/releases). Get the latest release of PhotonVison. The name of the file you download should end with `image_limelight.xy`. 

## Flash PhotonVision to limelight

Use the [Balena Etcher](https://www.balena.io/etcher/) software to flash the image onto the limelight. Connect your computer to the micro-USB of the limelight. The computer cannot be a Windows 7 or Windows XP. MAKE SURE THE LIMELIGHT HAS NO POWER. Then open Balena Etcher in adminstrator. After doing so, click the Flash From File button. Select the PhotonVision image you downloaded. Then click select target. Select the limelight. Then flash.

## Constants

Since PhotoVision's mathematical distance calculations are unreliable, we had to use mathematical modeling using `tuner.py`. We realize that PhotonVision's distance calculations are linearly related to the actual distance. We are inputting pitch and yaw into two separate linear functions. We have 4 constants: Aagrim's constant, Yajwin's constant, Aryav's constant, and Ritvik's constant.
Here is a breakdown of what they do:

Linear equation for pitch: $y = m_1x+b_1$ (where x is pitch)

Linear equation for yaw: $y = m_2x+b_2$ (where x is yaw)
* Aagrim's constant: The $m_1$ value for the **pitch** linear function 
* Yajwin's constant: The $b_1$ value for the **pitch** linear function
* Aryav's constant: The $m_2$ value for the **yaw** linear function
* Ritvik's constant: the $b_2$ value for the **yaw** linear function

### `tuner.py`

It is a python script that does some trig with the inputs. Using numpy it returns a linear equation that relates PhotonVision data to real values. To use, collect data on five differnt known distances away from AprilTag. Collect the following data for each distance:

* PhotonVision reported distance from tag
* PhotonVision reported yaw
* PhotonVision reported pitch
* Horizontal distance from robot to tag (manually measured)
* Actual distance from tag (manually measured)

//TODO: explain how to plug in values to `tuner.py`


## What is pitch?



