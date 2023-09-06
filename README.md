# Motion Detection Project with OpenCV and Python

This project is a motion detection system built using Python and the OpenCV library. It allows you to monitor a designated area (e.g., a room or outdoor space) using a video capturing device (such as a webcam or IP camera) and receive alerts when motion is detected. This README file provides an overview of the project and instructions on how to use it.

## Table of Contents

- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
- [Customization](#customization)

## Project Overview

Motion detection is a fundamental task in computer vision, and this project leverages the power of the OpenCV library to create a real-time motion detection system. The core functionality includes capturing video frames, detecting changes between consecutive frames, and alerting when motion is detected. It is a versatile solution with potential applications in home security, surveillance, wildlife monitoring, and automation.

## Key Features

- Real-time video frame capture.
- Frame differencing and thresholding to detect motion.
- Contour detection to identify areas of motion.
- Customizable sensitivity settings.
- Multiple alerting mechanisms, such as playing a sound, sending an email, or sending notifications.

## Requirements

To run this project, you'll need the following packages installed:

opencv-python==4.7.0.72: OpenCV is used for video capture, frame differencing, and contour detection.
To enable email alerts using Gmail APIs, you'll also need the following packages:

google-api-python-client: This package allows you to interact with Google APIs.
google-auth-httplib2: Provides authentication for HTTP requests made by the Google API client.
google-auth-oauthlib: Provides OAuth 2.0 authentication for the Google API client.

## Setup

1. Clone the project repository to your local machine:

```bash
git clone https://github.com/piyoush-jaiswal/Motion_Detection.git
```

2. Navigate to the project directory:

```bash
cd Motion_Detection
```

3. You can install the required packages using pip. Open a terminal and run the following commands:

```bash
pip install opencv-python==4.7.0.72
pip install google-api-python-client google-auth-httplib2 google-auth-oauthlib
```

## Usage

To use the motion detection system:

1. Run the main script:

```bash
python motion-dete2.py
```

2. The system will start capturing video frames and analyzing them for motion.

3. When motion is detected, the configured alert mechanism will be triggered (e.g., a sound will play, an email will be sent, or a notification will be generated).

4. Press `q` to exit the application.

## Customization

You can customize the motion detection system by modifying the following parameters in the `motion_detection.py` script:

- Sensitivity: Adjust the sensitivity threshold to control the level of motion detection.
- Alert Mechanism: Configure how you want to be alerted when motion is detected (e.g., change the sound file, email settings, or notification method).

Feel free to explore and modify the code to suit your specific requirements.
