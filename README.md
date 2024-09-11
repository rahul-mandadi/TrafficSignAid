# TrafficSignAid
Traffic Sign Assistant for Visually Impaired


---

# Traffic Sign Assistant for Visually Impaired

### Abstract

In today’s world, visually impaired individuals face significant challenges, especially when navigating urban environments and crossing roads. Our project, **Traffic Sign Assistant (TSA)**, addresses these challenges by leveraging advancements in assistive technology. The TSA enhances mobility and safety for visually impaired pedestrians by providing real-time recognition of traffic signs and delivering auditory feedback.

By empowering individuals with visual impairments, this tool facilitates independent navigation and lays the groundwork for further innovation in inclusive mobility solutions.

---

### Features

- **Real-time Traffic Sign Detection:** Utilizes advanced computer vision techniques (YOLO) to detect traffic signs from live camera feeds.
- **Classification of Traffic Signs:** A CNN-based model classifies recognized traffic signs.
- **Auditory Feedback:** Information about detected signs is communicated to the user via audio, ensuring a seamless, user-friendly experience.
  
---

### Technologies Used

- **YOLO (You Only Look Once):** For object detection.
- **Convolutional Neural Network (CNN):** For traffic sign classification.
- **Python**: Main programming language.
- **OpenCV**: For handling video input and image processing.

---

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/YourUsername/TrafficSignAid.git
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Ensure your camera or video input device is properly set up.

---

### Usage

1. Start the traffic sign detection:
    ```bash
    python run_TSA.py
    ```

2. The system will detect traffic signs in real-time and provide audio feedback to the user.

---

### Future Improvements

- **Tactile Feedback:** Integration of tactile methods to provide additional feedback.
- **Enhanced Accuracy:** Improving the model's recognition capabilities in varied weather and lighting conditions.
- **Broader Sign Database:** Expanding the range of recognizable traffic signs.


