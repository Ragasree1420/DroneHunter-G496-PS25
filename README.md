# AntiUAV600: Real-World UAV Detection and Tracking

## 📌 Project Introduction

AntiUAV600 is a large-scale thermal infrared dataset developed to train and evaluate anti-UAV (Unmanned Aerial Vehicle) systems in real-world conditions. It focuses on detecting and tracking small drones in dynamic environments without relying on prior template information. This project is motivated by the need for practical surveillance systems capable of handling unpredictable drone behavior in defense and civilian applications.

## 📖 Overview

- **Dataset Size**: 600 video sequences (300 training, 50 validation, 250 testing)
- **Frame Count**: Over 723,000 annotated thermal infrared frames
- **Challenges Addressed**:
  - Small UAV size
  - Complex and diverse backgrounds (e.g., sky, forest, city)
  - Random appearance and disappearance of UAVs in video frames
  - No requirement for template-based tracking
- **Annotations**: Bounding boxes for UAV presence, ‘Not Exist’ tag for absence
- **Attributes**: Occlusion, Fast Motion, Scale Variation, Out-of-View, etc.

## 🧠 Architecture 

The system uses an adaptive dual-branch approach:
- **Detection Branch**: Uses global search with a YOLO-style multi-scale head to detect UAVs in complex backgrounds.
- **Tracking Branch**: When confident, switches to local tracking using previously seen information to reduce computation.
- **Switching Logic**: Decides between detection and tracking based on confidence and evidential reasoning (uncertainty estimation).

## 🚀 Applications

- Military defense and border surveillance
- Public safety and smart city monitoring
- Critical infrastructure protection
- Wildlife protection and anti-poaching operations

## 👥 Users

- AI researchers in computer vision and tracking
- Defense and aerospace organizations
- Law enforcement agencies
- Smart city solution providers

## 🤝 Contributors

- Vaishnavi
- Sirivally
- Ragasree
- Sahasra
- Thahaseena


