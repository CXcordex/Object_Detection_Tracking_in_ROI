# Object_Detection_Tracking_in_ROI
This project implements a real-time object detection system to monitor and count people in predefined Regions of Interest (ROIs) within a video feed using YOLOv8, a state-of-the-art object detection model. The system is optimized for efficiency and can be deployed on live video feeds (e.g., from CCTV cameras) or prerecorded video files.
The main objective is to track the number of people present in specific zones, making it ideal for applications such as:

Crowd control and analysis,

Smart surveillance,

Social distancing monitoring,

Footfall analysis in retail or public areas.

🧠 Core Technologies Used
YOLOv8 (Ultralytics) – For fast and accurate object detection.

OpenCV – For video processing, ROI selection, and visual display.

NumPy – For array and coordinate manipulation.

TQDM – For displaying progress when processing video files.

Python – Main programming language.

🎯 Key Features
Real-time Detection: Detects people (class=0) frame by frame from live camera input.

Multiple ROIs: Allows defining multiple rectangular zones in the video frame.

Dynamic Count Overlay: Displays real-time counts of detected people in each ROI.

Customizable Parameters: Easily adjust frame scaling, confidence thresholds, and number of ROIs.

Video Output: Optionally saves the annotated output video with detection results.

🛠️ How It Works
Load YOLOv8 model pre-trained on the COCO dataset.

Capture video feed from a webcam or a video file.

Resize frames to improve processing speed.

Define multiple polygonal ROIs for monitoring specific areas in the frame.

Detect people (class 0) using YOLOv8 within each ROI.

Draw bounding boxes and ROI overlays, and count detections in each zone.

Display or save the output with real-time detection and counting data.

📸 Applications
Retail analytics – Count people in store sections.

Security surveillance – Monitor presence in restricted zones.

Event management – Track occupancy in event spaces.

Smart cities – Analyze public space usage.

✅ Requirements
Python 3.8+

OpenCV

Ultralytics (YOLOv8)

Webcam or video file input

🚀 Future Enhancements
Integrate with cloud dashboards for remote monitoring.

Add alert systems when counts exceed thresholds.

Enable drawing custom-shaped ROIs (not just rectangles).

Track individual identities using object tracking.
