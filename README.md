# DRONE HUNTER

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
The system follows a dual-branch architecture that combines a detection and tracking pipeline for robust UAV perception. The detection branch uses a YOLO-based multi-scale prediction head to identify UAVs in complex backgrounds. Once detected, the tracking branch—based on a Siamese network—continuously follows the UAV using relevance decoupling and evidential reasoning. The system adaptively switches between detection and tracking based on confidence levels, ensuring accurate and real-time monitoring even under occlusion, fast motion, and varying scales.
<img width="1137" height="505" alt="Screenshot 2025-07-29 134137" src="https://github.com/user-attachments/assets/a28ee78a-299e-4ffd-b689-f66dd8949fca" />


## 🧠 WorkFlow Diagram 
<img width="1044" height="582" alt="image" src="https://github.com/user-attachments/assets/4aac40cd-7b56-4e3f-8910-99c2de6d0e83" />


## 🚀 Why Agentic workflows
| 💼 **Feature**                      | 🔍 **Justification**                                                                 |
| ----------------------------------- | ------------------------------------------------------------------------------------ |
| **1. Adaptive Decision-Making**     | Automatically switches between detection and tracking based on current scene status. |
| **2. Dynamic Modality Switching**   | System dynamically decides whether to detect or track based on confidence scores.    |
| **3. Evidential Reasoning**         | Uses an Evidential Head to reason about uncertainty before deciding an action.       |
| **4. Goal-Oriented Behavior**       | Operates with a clear goal: continuous UAV localization regardless of visibility.    |
| **5. High Autonomy**                | Minimizes manual control; system self-manages based on UAV appearance patterns.      |
| **6. Real-Time Adaptability**       | Reacts to motion blur, occlusion, and sudden UAV re-appearance without reset.        |
| **7. Context-Aware Intelligence**   | Considers visibility, evidence, and confidence to select optimal branch.             |
| **8. Robustness in Complex Scenes** | Maintains performance even in sky, forest, urban, or river backgrounds.              |

### Tech Stack Used

| Component             | Description                                                       |
|----------------------|-------------------------------------------------------------------|
| Detection Backbone   | YOLO-based multi-scale prediction head (for initial UAV detection)|
| Tracking Module      | Siamese network with relevance decoupling for local tracking      |
| Framework            | PyTorch / TensorFlow (for model training and inference)           |
| Deployment Tools     | CUDA for GPU acceleration, OpenCV for video processing            |



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

👤 Name	🌐 GitHub Profile
Cheela Vaishnavi	@cheelavaishnavi123
Chandanala Sirivally	@sirivallych
Gaddam Ragasree	@Ragasree1420
Muddam Sahasra	@sahasra2617
Shaik Mahaboob Thahaseena	@Thahaseena0517



