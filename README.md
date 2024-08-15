# Car Counter Using YOLOv8 and SORT

## Overview

This project implements a real-time car counting system using the YOLOv8 object detection model and the SORT (Simple Online and Realtime Tracking) algorithm. The system detects cars in a video feed, assigns unique IDs to each vehicle, and tracks their movements across frames. The system also counts the number of cars that pass a designated line in the video.

## Features

- **Real-Time Car Detection**: Utilizes the YOLOv8 model for accurate and efficient car detection within video streams.
- **Object Tracking**: Implements the SORT algorithm to track detected vehicles with unique IDs, ensuring consistency across frames.
- **Car Counting**: Counts the number of vehicles that cross a predefined line in the video, updating the total car count in real-time.
- **OpenCV Integration**: Leverages the powerful OpenCV library for video processing and drawing utilities.

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/sritarung/Car-counter.git
   cd Car-counter
   ```

2. **Install dependencies:**

   Make sure you have Python installed (preferably Python 3.8 or higher). Install the required Python packages using `pip`:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Prepare your video file:**

   Ensure your input video is placed in the `input/` directory. Update the `video_path` variable in the script with the path to your video file.

2. **Run the car counter:**

   Execute the main script to start the car counting process:

   ```bash
   python car_counter.py
    ```

3. **View the reuslts**

## Configuration

- **Line Position:** You can modify the line position for counting cars by adjusting the coordinates in the script. This line acts as a reference to determine when a car has passed and should be counted.
- **Tracking Parameters:** SORT algorithm parameters can be tuned within the script to improve tracking performance based on your specific video feed.

## Future Improvements

- **Multiple Class Tracking:** Extend the system to detect and track different types of vehicles (e.g., trucks, motorcycles).
- **Speed Estimation:** Implement speed estimation for tracked vehicles.
- **Performance Optimization:** Explore optimizing the detection and tracking pipeline for faster processing times on lower-end hardware.

## Acknowledgments

- **YOLOv8:** [Ultralytics YOLOv8](https://github.com/ultralytics/yolov8) for the object detection model.
- **SORT Algorithm:** [SORT](https://github.com/abewley/sort) for real-time tracking.


