# Parking Vision: AI Eyes on Every Spot

## Project Overview
This project leverages computer vision and drone technology to solve parking management challenges. By integrating a Tello drone with a custom-trained object detection model, the system provides real-time monitoring to determine if parking spaces are "Occupied" or "Empty" [1, 4]. The solution is designed to be scalable, easy to deploy, and effective in outdoor environments where traditional sensors are too costly [4].

## The Challenge
We initially attempted to use models trained on publicly available datasets, but results were consistently suboptimal due to local environmental factors [5]. Specifically, the target parking lot used circular ground markings rather than traditional painted lines, which confused standard models [6].

## Methodology & Technologies
*   **Hardware:** Tello Drone (for testing/overhead views) and Smartphones (for data collection) [6].
*   **Model:** YOLOv8s (You Only Look Once), chosen for its object detection capabilities [2].
*   **Tools:** Visual Studio for training, Roboflow for annotation [2].
*   **Pipeline:**
    1.  **Data Collection:** Manually captured images of local parking lots using smartphones and drones to ensure variety in angles and lighting [2, 6].
    2.  **Preprocessing:** Manually annotated images and applied augmentation (rotation, flipping, brightness changes) to expand the dataset [2].
    3.  **Training:** The model was trained over 2.5 hours [3].

## Results
The model was tested in real-world scenarios with live drone footage, yielding high-performance metrics:
*   **Precision:** 99% [3]
*   **mAP (Mean Average Precision):** 75% [3]
*   **Recall:** 64% [3]

The system successfully detected and classified parking spots in real-time during flight tests [3].

## Key Learnings & Future Work
*   **Data Quality:** We learned that data collected from the actual target environment is more critical for accuracy than the sheer quantity of generic data [7].
*   **Challenges Overcome:** The project navigated hardware limitations, including drone overheating and poor camera stabilization [8].
*   **Future Improvements:** Plans include adding functionality to detect "wrong parking" (e.g., taking two spots), classifying vehicle types (cars vs. trucks), and implementing drone-assisted guidance for drivers [9].

--------------------------------------------------------------------------------
