# 🚗 Smart Lane Detection & Direction Prediction

A real-time lane detection and direction prediction system using OpenCV and Python. This AI-powered project identifies road lanes from video or webcam feed and intelligently predicts the movement direction: ⏩ Going Straight, ↩️ Turning Left, or ↪️ Turning Right.

---

## 🔍 Features

- 🎥 Lane detection from live camera or video input
- 🧠 Direction prediction using lane slope logic
- 🗣️ Voice output (via `pyttsx3` on local systems)
- 🖼️ Region of Interest (ROI) for focused detection
- 📦 Clean modular structure and easy integration

---

## 🛠️ Tech Stack

- Python 3.x 🐍
- OpenCV (Computer Vision) 🎥
- NumPy (Math operations) ➕
- Pyttsx3 (Text-to-Speech, optional) 🔊

---

## 🚀 How to Run

### 🔧 Installation

```bash
pip install opencv-python numpy pyttsx3
````

⚠️ Note: `pyttsx3` works only on local machines (not on Google Colab). In Colab, just use `print()` instead.

---

### 🧪 Running the Code

#### ▶️ With Webcam

```python
cap = cv2.VideoCapture(0)
```

#### 📼 With Saved Video

```python
cap = cv2.VideoCapture("synthetic_lane_video.avi")
```

---

### 🗣️ Optional: Voice Feedback

Enable this for real-time audio output (local only):

```python
import pyttsx3

engine = pyttsx3.init()
engine.say("Turning Left")
engine.runAndWait()
```

---

## 📁 Project Structure

```
📦 lane_detection_project/
├── lane_detection.ipynb       # Jupyter notebook for lane prediction
├── synthetic_lane_video.avi   # Sample generated lane video
├── lane1.jpeg, lane2.jpeg     # Sample input frames
├── sequence diagram.png       # Diagram for architecture
└── README.md                  # You're here 😎
```

---

## 📈 Direction Prediction Logic

* Uses **Hough Line Transform** to extract lane lines.
* Calculates **slope** of left and right lines.
* Based on slope angles:

  * 🔄 Left turn → steep left slope
  * ⏩ Straight → opposite equal slopes
  * 🔃 Right turn → steep right slope

---

## 🚧 Future Scope

* Polynomial curve detection (curved roads)
* YOLO integration for obstacle detection
* Real-time lane change alerts with dashboard
* Deploy as Android app or Web visualizer

---

## 🤝 Contributions

Pull requests are welcome! Feel free to fork and improve.

---

## 👨‍💻 Author

**Lokesh Agarwal**
📧 [lokeshagarwal2304@gmail.com](mailto:lokeshagarwal2304@gmail.com)
🔗 [LinkedIn](https://www.linkedin.com/in/lokeshagarwal2304)
📸 [Instagram](https://instagram.com/_lokesh._.agarwal_)

---

## 📜 License

This project is licensed under the **MIT License** – use it freely with credit 🙌

```

---

Bhai agar tu chahta hai ki main isme ek preview GIF/video, badges (build, license, version) ya AI model integration section bhi add karu, toh bol de — turant ready!
```
