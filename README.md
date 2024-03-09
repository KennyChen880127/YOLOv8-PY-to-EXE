# Convert-YOLOv8-PY-to-EXE
This project aims to demonstrate how to convert YOLOv8 Python files (.py) into executable files (.exe) using Pyinstaller.

## Pyinstaller
[PyInstaller](https://pyinstaller.org/en/stable/) bundles a Python application and all its dependencies into a single package. The user can run the packaged app without installing a Python interpreter or any modules. PyInstaller supports Python 3.8 and newer, and correctly bundles many major Python packages such as numpy, matplotlib, PyQt, wxPython, and others.

## Steps to run Code
### Create Virtual Environment
* Create and activate a virtual environment using Anaconda:

        conda create --name yolov8 python=3.8 -y
        conda activate yolov8

* Install the required packages:

        pip install pyinstaller ultralytics opencv-python

* Download the YOLOv8 library.

        git clone https://github.com/ultralytics/ultralytics.git

* After editing the program, open the terminal and navigate to the project directory:
        
        pyinstaller main.py --onefile --add-data "ultralytics;."
  
#### Result
![result](https://github.com/KennyChen880127/YOLOv8-PY-to-EXE/blob/master/result.jpg)
