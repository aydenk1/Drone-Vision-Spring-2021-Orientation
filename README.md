# Drone-Vision-Spring-2021-Orientation

## Step 1. Setup Linux Environment
Working in a linux environment will be essential to running software for the drone vision team. There are many ways to achieve this, with tons of ways to mess up as well. Please   feel free to ask Justin or I if you run into problems.

### Creating a Linux Environment
- Windows
  - Dual Booting: Prefered Method, but harder. ~1 TB storage and 8 GB Flash Drive are required
    - Please read this article, which helps to explain how to [dual boot](https://www.howtogeek.com/214571/how-to-dual-boot-linux-on-your-pc/). I recommend Kubuntu 20.04.1 LTS, because it is the most easy to use in my opinion.
  - Windows Subsystem for Linux (WSL)
    - Installation tutorial for [WSL](https://docs.microsoft.com/en-us/windows/wsl/install-win10). Ubuntu will be the distro you should install.
- MacOS
  - Install [VirtualBox](https://www.virtualbox.org/wiki/Download).
  - Linux install for [VirtualBox tutorial](https://www.imore.com/how-use-linux-your-mac-using-virtual-machine). 
### Installing Miniconda
- Installation Tutorial for [Miniconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html). Miniconda will be useful, since it allows you to create separate python environments and makes debugging easier. Verify Miniconda is working properly by the following code and update if needed.
  ```
  conda update conda
  ```


## Step 2. Perform object detection
- Clone this repo and setup [YoloV5](https://github.com/ultralytics/yolov5)
  - Since many programs require different versions of dependencies, it is good practice to setup YoloV5 in a virtual environment. To do this, create an environment named YoloV5 with Python 3.8 installed. Then, activate the environment. Run the following code to create and activate the environment:
    ```
    conda create --name YoloV5 python=3.8
    conda activate YoloV5
    ```
  
- Download the [sample video](https://purdue0-my.sharepoint.com/:v:/g/personal/hu440_purdue_edu/EbxwYJGdvipLqD1r4WzTknwBkDALLMGRGWuXv2amaM5Y7g?e=Kgg1co) and run Yolov5 to generate detections.
  - Use the Yolov5l weights.
### We will be testing the accuracy of the detections that are generated, and should be equal to the base Yolov5l weights. 


