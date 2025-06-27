
markdown
Copy
Edit
# 🚁 AI-Powered Drone for Smart Parking Detection

## 👨‍💻 Team Members
- **Mohammed Omar Halawani**-(STEELWARDEN)-
- **Mohammed Almansour**-(covu0)-
- **Naif Almasoud**-(CodeNaif)-
- **Ahmed Al-Ghamdi**-(I think it's clear)-

---

## 📌 Project Overview

This project addresses a real-world urban challenge: **finding available parking spaces**. We built a system using a **Tello drone** and an **AI-based object detection model (YOLOv8)** to detect and classify parking spots as **occupied** or **empty** in real time. 

Our solution is designed to be **scalable, mobile, and adaptable**, ideal for locations where traditional sensors are impractical.

---

## 📷 Data Collection

- We created our own **custom dataset** using smartphone and drone images.
- Images were taken from **multiple angles**, lighting conditions, and distances.
- Parking spots in our location are **marked with circular ground markers**—making existing public datasets ineffective.
- We **manually annotated** each image using [Roboflow](https://roboflow.com/).
- Data augmentation included: rotation, flipping, brightness variation, etc.
-NOTE:[We cannot upload our dataset due to the legal issues about license plates].

---

## 🧠 Model Training

- Model used: `YOLOv8s` (You Only Look Once v8 - small version)
- Platform: **Visual Studio Code** with **Python**
- Dataset Size: Images from various parking areas
- Labels: `empty`, `occupied`
- Training time: ~2.5 hours
- Training involved annotation and augmentation using Roboflow tools

---

## 🧪 Testing & Results

- Tested the model on **real-life images** and during **live drone flights**
- Achieved:
  - 🔍 **Precision**: 99%
  - 🔁 **Recall**: 64%
  - 📊 **mAP (mean average precision)**: 75%
- The model successfully identified and classified parking spots **in real time**

---

## ⚠️ Challenges Faced

1. **Dataset Limitations**: Public datasets were not effective; we had to create our own.
2. **Manual Annotation**: Very time-consuming but necessary for accuracy.
3. **Hardware Constraints**: Real-time detection required high computational power.
4. **Drone Issues**: Tello drone often overheated or shut down unexpectedly.
5. **Camera Quality**: Low resolution and poor stabilization reduced detection accuracy.

---

## 🚀 Future Improvements

- ❌ **Wrong Parking Detection** – Detect violations like double parking or blocking.
- 🚗 **Vehicle Type Classification** – Differentiate between cars, trucks, motorcycles, etc.
- 🧭 **Drone-Assisted Parking Guidance** – Help vehicles find spots using real-time drone visuals.
- 🧠 **Model Accuracy Enhancement** – Gather more diverse and high-quality data.

---

## 💡 Why This Project?

- ✅ **Real-Time Monitoring** – Live feedback on parking availability.
- 🔄 **Scalable** – Easily redeployable in new locations.
- 🏗️ **Infrastructure-Free** – No need for fixed sensors or major installations.
- 📈 **Insightful Data** – Provides analytics like usage trends and peak hours.

---

## 📚 What We Learned

This project taught us the power of combining **AI and robotics** to address urban challenges. Key takeaways include:

- Effective **data selection** is more important than sheer data quantity.
- **Custom, context-specific data** dramatically improves model performance.
- **Integrating drones** with AI systems unlocks new possibilities for automation and monitoring.

---

## 🎥 Demo / 

[watch the demo!]->(https://drive.google.com/file/d/1l6NDHIehwuwdhlFE9Pbl5tkEanyvBgME/view?usp=drive_link)
---

## 🙏 Acknowledgements

Special thanks to our instructors and all contributors who supported this journey. Tools used:
- Roboflow
- Ultralytics YOLOv8
- Python, OpenCV
- DJI Tello Drone

---
