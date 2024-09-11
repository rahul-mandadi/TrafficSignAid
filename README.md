
# Traffic Sign Assistant for Visually Impaired Pedestrian

### Abstract

Visually impaired individuals face significant challenges when navigating urban environments, especially when crossing roads. The **Traffic Sign Assistant (TSA)** is designed to help visually impaired pedestrians by utilizing cutting-edge computer vision techniques to detect traffic signs in real-time and provide auditory feedback. The system integrates YOLO-based object detection and Convolutional Neural Networks (CNN) for classification, ensuring safe and independent mobility.

---

### Features

- **Real-time Traffic Sign Detection:** Uses the YOLOv8 model for detecting traffic signs from live video feeds.
- **Accurate Traffic Sign Classification:** Employs CNN-based models (ResNet50, DenseNet, VGGNet) to classify detected signs.
- **Auditory Feedback:** Converts detected traffic sign information into speech using Google Text-to-Speech (GTTS) for real-time audio guidance.

---

### Achievements

- **Detection Accuracy:** Achieved an outstanding detection accuracy of **97.62%** using the YOLOv8 object detection model.
  
- **Processing Speed:** The system runs at an average of **25 FPS**, ensuring smooth and real-time video processing.
  
- **Classification Accuracy:** The CNN-based classification system has a classification accuracy of **97.62%** across various traffic sign categories.

- **Diverse Dataset Support:** The model is trained on a custom dataset with 1.6k images for object detection and the **GTSRB dataset** (52,000 images) for traffic sign classification.

- **Real-Time Auditory Feedback:** The system provides auditory feedback within **300 milliseconds**, allowing the visually impaired to receive prompt navigation cues.

---

### Datasets Used

- **Custom Traffic Sign Dataset:** This dataset contains 1.6k images, categorized into four classes: Prohibited, Danger, Mandatory, and Other. It is used to train the YOLOv8 model for object detection.
  
- **GTSRB (German Traffic Sign Recognition Benchmark):** A widely-used dataset of over 50,000 images across 43 categories of traffic signs, utilized for CNN model training in traffic sign classification.

---

### Classifiers Explored

The following classifiers were implemented and evaluated for traffic sign classification, with the respective accuracy rates:

1. **CNN (Convolutional Neural Network):** Achieved a remarkable accuracy of **97.62%**, proving to be the top performer for traffic sign classification .

2. **VGGNet:** Although it offers a deep network structure, VGGNet reached an accuracy of **80.89%**, but it was less efficient due to its high computational resource demands .

3. **ResNet50:** By using residual connections to improve gradient flow, ResNet50 achieved a competitive accuracy of **93.78%**, offering a balance between performance and complexity .

4. **DenseNet:** DenseNet, known for its dense connectivity, demonstrated strong performance with an accuracy of **94.55%**, enabling efficient feature reuse and better gradient propagation .

---

### Object Detection: YOLO Model

The **YOLOv8** model was employed for real-time traffic sign detection, and it processes video frames while generating bounding boxes around detected signs. These bounding boxes are passed to CNN-based classifiers for further sign classification.

- **Feature Extraction:** YOLOv8 extracts low-level and high-level features from input video frames, allowing for real-time detection of traffic signs.
- **Multi-Scale Feature Fusion:** The model fuses features from different scales and resolutions, ensuring accurate detection of both large and small signs.
- **Bounding Box Generation:** YOLOv8 generates bounding boxes around traffic signs in real-time, providing precise localization.

---

### Installation

To set up the Traffic Sign Assistant, follow these steps:

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/YourUsername/TrafficSignAid.git
    ```

2. **Run the Program:**
    Ensure your camera or video input is connected and run:
    ```bash
    python run_TSA.py
    ```

---

### Usage

- Once the system is running, it will detect traffic signs in real-time from the video feed.
- The system provides auditory feedback about the detected signs to the user, aiding navigation.

---

### Future Enhancements

- **Tactile Feedback:** Future work could integrate tactile feedback to supplement auditory feedback for users.
  
- **Expanded Dataset Coverage:** Additional datasets will be explored to enhance the system’s performance across different countries and sign systems.
  
- **Improved Robustness:** Enhancements in the system’s ability to perform in challenging conditions such as low-light, poor weather, and occlusions will be implemented.

- **Model Optimization:** Further optimization of both YOLOv8 and CNN models to increase performance and reduce resource consumption.

---

### Testing and Evaluation

- **Metrics Used:** The performance of the detection and classification models was evaluated using mAP (mean Average Precision) and mAP50-95.
  
- **Testing Environment:** The system was tested in both controlled environments using video feeds and with real-world inputs, ensuring robust performance under varied conditions.

---
