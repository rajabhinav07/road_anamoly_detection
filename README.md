# road_anamoly_detection
Real-time pothole detection system optimized for Raspberry Pi 4. Uses an INT8-quantized YOLO model via TensorFlow Lite with automatic aspect-ratio correction and CSV event logging.

Markdown

# 🚗 Real-Time Pothole Detector

A lightweight computer vision system designed to detect road potholes in real-time. This project uses a custom-trained, INT8-quantized YOLO model running via TensorFlow Lite. 

It processes live feeds from a webcam or uploaded video files, logs detections to a CSV file, and displays a live confidence and FPS overlay.

##  Project Structure
* `main.py`: The main Python script to run the detector.
* `best-int8.tflite`: The quantized neural network model.
* `my_project_venv/`: The virtual environment containing required Python libraries.
* `pothole_events.csv`: The auto-generated log file of detected potholes.
* `test_vid2.mp4`: Sample video for testing.

##  How to Run

### 1. Download and Open
1. Download or clone this repository to your computer.
2. Open the `pothole-detector` folder.
3. Right-click inside the folder and select **Open in Terminal** (or open Command Prompt and `cd` to this folder).
   

### 2. Activate the Virtual Environment
Before running the script, you must activate the environment where your libraries are installed.

* **If using Command Prompt (cmd.exe):**
  my_project_venv\Scripts\activate.bat

  
If using PowerShell:
   my_project_venv\Scripts\Activate.ps1

   
If using Git Bash:
   source my_project_venv/Scripts/activate
(You will know it worked when you see (my_project_venv) appear at the beginning of your terminal line).

3. Run the Detector
With the environment active, start the program:

Bash

python main.py
4. Select Your Mode
The terminal will prompt you to choose an input method:

Press 1 for Live Camera (Webcam).

Press 2 for Video File. It will ask for the filename (e.g., type test_vid2.mp4 and press Enter).
