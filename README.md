# 🧠 Face Recognition & Emotion Detection (Real-Time)

This project uses **MTCNN** for face detection, **Facenet (InceptionResnetV1)** for face recognition, and **DeepFace** for emotion detection in real-time using a webcam.

---

## 📌 Features

- 🧍 Detects and identifies multiple known faces per frame.
- 🎭 Recognizes dominant emotions like happy, sad, angry, etc.
- 🧠 Uses deep learning-based **Facenet** embeddings for accurate recognition.
- 🎥 Real-time webcam video capture.
- 🚫 Avoids duplicate detections within a single frame.
- ✅ Handles multiple faces per frame (configurable).

---

## 🛠️ Technologies Used

- Python
- OpenCV
- PyTorch
- Facenet-PyTorch
- DeepFace
- scikit-learn

---

## 📁 Folder Structure
project/
│
├── known_faces/ # Folder containing subfolders of known persons with images
│ ├── person1/
│ │ ├── img1.jpg
│ │ ├── img2.jpg
│ ├── person2/
│ ├── img1.jpg
│ └── img2.jpg
│
├── main.py # Main Python script
└── README.md # Project documentation

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
2. Install dependencies
bash
Copy
Edit
pip install opencv-python torch torchvision facenet-pytorch deepface scikit-learn
3. Add known faces
Place images of each person in separate folders inside the known_faces directory.

Example:

Copy
Edit
known_faces/
├── Alice/
│   ├── img1.jpg
│   └── img2.jpg
└── Bob/
    └── img1.jpg
4. Run the script
bash
Copy
Edit
python main.py
⚙️ Configuration
SIMILARITY_THRESHOLD - Controls how strict face matching is (default: 0.6)

MAX_FACES_PER_FRAME - Limits number of faces processed per frame (default: 5)

📌 Notes
DeepFace works best with clear, front-facing faces.

Ensure good lighting and size of known faces for reliable recognition.

MTCNN works with CPU but performs better with GPU (CUDA).

🛡️ License
This project is for educational purposes. Modify and use it as needed.

---

Let me know if you want me to include a `requirements.txt` or a sample known face folder.
