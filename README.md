# E - learning with smart phone 

a sample android app with face recognition for IT training of students via teacher and a PHP backend.

# First App: 📌 MyFaceRecognizer

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

# Second App: 📸 CaptureImage

This module provides a simple Python script that captures images from a webcam and saves them to disk for use in the Elearning-with-Smart-Phone project. It’s designed as a building block for later tasks such as face recognition, dataset creation, and training models.

The script uses OpenCV, a popular computer vision library, to access the webcam and detect frames, allowing users to save images interactively.

🧠 Overview

In many computer vision and face recognition workflows, collecting a dataset of face images is the first step. This module:

🖼️ Captures images from your webcam

📁 Saves them into a specified directory

📋 Helps you generate training data (e.g., for facial recognition or classification models)

This is similar to other webcam image capture tools that use OpenCV for real-time capture and storage of image frames.

📁 Project Structure
CaptureImage/
├── capture_images.py      # Main script for capturing images
├── output/                # Saved images (created after capture)
├── requirements.txt       # Dependencies required
└── README.md              # This file

Your directory structure may vary slightly based on additional files you include.

📦 Requirements

Before running the script, make sure you have the following:

Python 3.x

OpenCV (opencv-python)

Other packages in requirements.txt

You can install all requirements using:

pip install -r requirements.txt
🛠️ Installing & Setup

Clone the parent repository:

git clone https://github.com/imrankhan15/Elearning-with-Smart-Phone.git
cd Elearning-with-Smart-Phone/CaptureImage

Install dependencies:

pip install -r requirements.txt
🚀 How to Use

Run the capture script to start capturing images from your webcam:

python capture_images.py
📸 Interactive Controls

The script typically works like this (assuming typical implementation):

📷 The webcam feed will open in a window.

👤 When the desired subject is in frame, press a key (e.g., s) to save the current image.

🛑 Press another key (e.g., q) to quit the capture session.

You’ll find saved images inside the designated output folder (e.g., output/). These images can be used later for training models, building datasets, or running recognition scripts.

Note: Make sure your environment has webcam access.

🧩 Tips for Better Capture

✔ Ensure good lighting and stable positioning for clear images.
✔ Increase the number of images per subject for better model training.
✔ Name the saved files systematically (e.g., name + timestamp).

🔄 What’s Next?

After you’ve captured enough images, you can:

Use them to train a face recognizer.

Integrate them into the Myfacerecognizer module of this project.

Run recognition and testing using real-time detection.

🤝 Contributing

Contributions are welcome! If you have enhancements (e.g., better UI, automated capture loops, improvements for lighting conditions), feel free to open an issue or submit a pull request.

# 📡 Server – Elearning with Smart Phone

This directory contains the backend server for the Elearning-with-Smart-Phone project. It implements a RESTful API that handles data and business logic for the e-learning platform, such as user authentication, course data, and interactions with the mobile app.

A REST API (Representational State Transfer) is an HTTP-based web service that allows clients (mobile apps, web apps, etc.) to communicate with the server using defined endpoints and JSON data formats. This architecture helps decouple frontend and backend development for better scalability and maintenance.

🚀 Features

Depending on your implementation, the server may include:

🧑‍💻 User Authentication & Authorization
Login, signup, secure access control

📚 Course Management
Endpoints for creating, editing, deleting, and retrieving courses

👩‍🎓 Student & Instructor Profiles
User information, roles, and permissions

📝 Content Delivery
APIs for delivering course materials (text, media, assignments)

📊 Progress Tracking
Track user progress and completion status

🔐 Secure REST API using stateless authentication tokens
(JWT or similar) for scalable mobile integration

Update this list with specifics from your server code (e.g., routes, middleware) to reflect exactly what endpoints exist.

📁 Project Structure

Here’s a typical structure for a REST API backend:

server/
├── controllers/          # Logic for each API route
├── models/               # Database models or schemas
├── routes/               # API endpoint definitions
├── middleware/           # Authentication & utility middleware
├── config/               # Configuration files (DB, secrets)
├── app.js / server.js    # Entry point for the server
├── .env                  # Environment variables
├── package.json          # Dependencies & scripts
└── README.md             # This file

Adjust folder names and contents based on your actual project.

🛠️ Requirements

Before you start, make sure you have installed:

Node.js (if using Node backend)

Database (e.g., MongoDB / PostgreSQL / MySQL)

Environment variables configured (e.g., API keys, DB connection)

📦 Setup & Installation

Clone the repository:

git clone https://github.com/imrankhan15/Elearning-with-Smart-Phone.git
cd Elearning-with-Smart-Phone/server

Install dependencies:

npm install

Configure environment variables:

Create a .env file and add:

PORT=5000
DB_URI=<your_database_connection_string>
JWT_SECRET=<your_jwt_secret>

Run the server:

npm start

The API will start listening on the configured port (e.g., http://localhost:5000
).

📡 API Endpoints

Here’s a general idea of how typical REST endpoints might look. Update these according to your implementation:

Method	Endpoint	Description
POST	/auth/signup	Register a new user
POST	/auth/login	User login
GET	/courses	List all courses
POST	/courses	Create a new course
GET	/courses/:id	Get a single course
PUT	/courses/:id	Update course
DELETE	/courses/:id	Delete course

These patterns follow standard REST API practices for e-learning servers.

🔒 Security

Make sure your server includes:

Token-based authentication (e.g., JWT)

Input validation & error handling

Secure storage of credentials

Proper CORS configuration

These help protect user data and ensure your API is safe for production use.

🧪 Testing

Use tools like Postman or Insomnia to test your API endpoints. You can also include automated tests using frameworks like Jest or Mocha.

🤝 Contributing

Contributions are welcome! ✨

Fork the repo

Create a new branch (git checkout -b feature-name)

Make your changes

Submit a Pull Request
