 AI-Powered Traffic Management System
An intelligent traffic management system that uses AI-powered cameras to dynamically control traffic signals and prioritize emergency vehicles like ambulances and police cars. This project aims to reduce traffic congestion and decrease response times for emergency services.

✨ Features
Dynamic Signal Control: Automatically adjusts traffic light timings based on real-time vehicle density at intersections.

Emergency Vehicle Detection: Identifies ambulances and police vehicles using a custom-trained deep learning model (e.g., YOLOv8).

Green Corridor Creation: Automatically turns signals green along the path of a detected emergency vehicle to provide a clear route.

Real-Time Monitoring: A dashboard provides a live view of traffic flow and system status.

Data Analytics: Collects and analyzes traffic data to identify congestion patterns and optimize traffic flow over time.

⚙️ How It Works
The system follows a simple yet effective workflow to manage traffic and prioritize emergency vehicles.

Capture: IP cameras or webcams installed at intersections capture a live video feed of the traffic.

Detect & Classify: The video feed is processed by a deep learning model (YOLO) running on a local server or edge device. The model detects and classifies objects in real-time, identifying cars, trucks, buses, motorcycles, ambulances, and police vehicles.

Analyze: The system calculates vehicle density for each lane and detects the presence of any emergency vehicles.

Control:

Based on vehicle density, the algorithm intelligently allocates green light time to reduce congestion.

If an ambulance or police vehicle is detected, the system overrides the normal cycle and creates a "green corridor" by turning the traffic lights green in its direction and red for all other conflicting lanes.

Reset: Once the emergency vehicle has passed the intersection, the system returns to its normal, density-based operation.
