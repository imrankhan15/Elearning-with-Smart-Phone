# E - learning with smart phone 

a sample android app with face recognition for IT training of students via teacher and a PHP backend.

📌 MyFaceRecognizer

A simple face detection and recognition tool built with Python and OpenCV as part of the Elearning-with-Smart-Phone project. This module captures faces from a live camera feed, trains a recognizer, and identifies known faces in real time.

👇 Add installation, usage, and contribution instructions below.

🚀 Features

📸 Real-time face detection from webcam or live video.

🧠 Face recognition using trained images.

🗂️ Capture and save new face datasets.

🏷️ Recognize faces with labeled identities.

🧩 How It Works

This project uses computer vision techniques to:

Detect faces in camera input using Haar Cascades or similar classifier files.

Collect face images and generate a dataset for training.

Train a face recognizer model on collected data.

Recognize and display person identities in real time.

📁 Project Structure
Myfacerecognizer/
├── dataset/                  # Collected face images
├── classifier/               # Trained recognizer models
├── haarcascade/              # Pretrained detection models
├── capture_faces.py          # Capture images for training
├── train_recognizer.py       # Train recognition model
├── recognize_faces.py        # Run real-time recognition
├── requirements.txt          # Python dependencies
└── README.md

Adjust paths and filenames based on your project’s actual content.

🛠️ Requirements

Before running the project, make sure you have the following installed:

Python 3.x

OpenCV

NumPy

Other dependencies listed in requirements.txt

You can install them using:

pip install -r requirements.txt
📥 Installation

Clone the repository:

git clone https://github.com/imrankhan15/Elearning-with-Smart-Phone.git
cd Elearning-with-Smart-Phone/Myfacerecognizer

Install dependencies:

pip install -r requirements.txt
🧠 Usage
1. Capture Face Images

Run the capture script to collect images of a person:

python capture_faces.py

Follow the on-screen prompts to save images into the dataset.

2. Train Recognizer

Train the face recognition model using your dataset:

python train_recognizer.py
3. Run Real-Time Recognition

Start the face recognition interface:

python recognize_faces.py

Use your webcam and see recognized faces with labels.

🧪 Sample Output

Once running, the application:

✔ Shows a live camera feed
✔ Detects faces and displays bounding boxes
✔ Recognizes trained faces and shows labels

📌 Tips

Add more face samples per person for better accuracy.

Ensure good lighting and clear face images while capturing.

Adjust camera resolution for performance and accuracy balance.

🤝 Contributing

Contributions are welcome! If you have suggestions or improvements (e.g., GUI, better models, mobile integration), feel free to open an issue or submit a pull request.
this project was developed in 2013-14 as part of BUET undergrad thesis demo app.
