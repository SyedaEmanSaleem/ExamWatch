
# 🎯 ExamWatch: Cheating Detection using YOLO11m Pose Estimation

**ExamWatch** is an AI-powered system that detects suspicious student behavior such as **looking sideways or potential cheating** during classroom or online examinations.
Using **YOLO11m Pose Estimation**, it tracks **head pose angles (yaw and pitch)** to distinguish between **focused** and **suspicious sideways glances**, ensuring exam integrity through **computer vision** and **deep learning**.

---

## 🧠 Features

* 🎥 Real-time detection of **student head movement and posture**
* 🧍 Tracks **yaw (left–right)** and **pitch (up–down)** angles
* 🕵️ Detects **focused** and **suspicious** head orientations
* 📊 Produces **annotated video output** with visual alerts
* ⚡ Built with **YOLO11m Pose**, **OpenCV**, and **cvzone**

---

## 🧰 Tech Stack

| Component       | Description                 |
| --------------- | --------------------------- |
| **Model**       | YOLO11m Pose (Ultralytics)  |
| **Framework**   | Python                      |
| **Libraries**   | OpenCV, cvzone, NumPy, math |
| **Environment** | Google Colab / VS Code      |

---

## ⚙️ Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/SyedaEmanSaleem/ExamWatch.git
cd ExamWatch
```

### 2️⃣ Install dependencies

```bash
pip install ultralytics opencv-python cvzone numpy
```

### 3️⃣ Download YOLO11m Pose Model

```python
from ultralytics import YOLO
model = YOLO('yolo11m-pose.pt')
```

### 4️⃣ Run the project

```bash
python examwatch.py
```

---

## 🧩 How It Works

1. The **YOLO11m Pose model** detects students and extracts body keypoints (nose, eyes, shoulders).
2. The system calculates **yaw** (left–right) and **pitch** (up–down) angles for each detected student.
3. Based on these angles, it classifies head movement as:

| Classification      | Behavior                                          | Indicator |
| ------------------- | ------------------------------------------------- | --------- |
| 🟢 Focused          | Head facing forward/downward (normal behavior)    | ✅ Green   |
| 🔴 Looking Sideways | Head turned beyond threshold (potential cheating) | ⚠️ Red    |

🎥 The annotated video output displays detections in **real-time**.

---

## 🖼️ Example Output

| Focused | Looking Sideways |
| ------- | ---------------- |
| ✅ Green | ⚠️ Red           |

---

## 📦 Requirements

* Python ≥ 3.8
* OpenCV
* cvzone
* ultralytics
* numpy

---

## 🚀 Future Enhancements

* 👁️ Add **eye gaze estimation** for higher accuracy
* 🧠 Apply **temporal filters** to smooth pose variations
* 🌐 Enable **real-time webcam monitoring**
* 📈 Develop a **dashboard for live analytics**

---

## 🧑‍💻 Author

**Syeda Eman Saleem**
[GitHub](https://github.com/SyedaEmanSaleem) • [LinkedIn](#)

---

## 🏷️ License

Released under the **MIT License** — free to use, modify, and distribute.

---

### 🔖 Hashtags

#AIProjects #ComputerVision #YOLO11 #DeepLearning #PoseEstimation #ExamProctoring #CheatingDetection #MachineLearning #OpenCV #Ultralytics #Python #ExamWatch

