
# 🏋️SmartFitness-AI

An **AI-powered fitness assistant** that analyzes user health data and activity history to predict fitness level, estimate calories burned, and generate personalized workout recommendations with interactive 3D exercise guidance.

---

[![Python](https://camo.githubusercontent.com/8d7c0956f2425d54cbe8fcefae0646c58d79f0d60e27403a3a26d7b0b50cb5fe/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f507974686f6e2d332e31302d626c7565)](https://camo.githubusercontent.com/8d7c0956f2425d54cbe8fcefae0646c58d79f0d60e27403a3a26d7b0b50cb5fe/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f507974686f6e2d332e31302d626c7565) [![DVC](https://camo.githubusercontent.com/9c645314947605669f54ccff100d6f2cc5aac21ea6cc5ae276ae3825793952f0/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4456432d322e302b2d6f72616e6765)](https://camo.githubusercontent.com/9c645314947605669f54ccff100d6f2cc5aac21ea6cc5ae276ae3825793952f0/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4456432d322e302b2d6f72616e6765) [![MLflow](https://camo.githubusercontent.com/d5eb3f7204eeb1e44a89f27ba746fecf8727e0323e92ad64ef81715b02b78c6c/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4d4c666c6f772d547261636b696e672d79656c6c6f77)](https://camo.githubusercontent.com/d5eb3f7204eeb1e44a89f27ba746fecf8727e0323e92ad64ef81715b02b78c6c/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4d4c666c6f772d547261636b696e672d79656c6c6f77) [![AWS S3](https://camo.githubusercontent.com/c36b22f42553605bb62b3dd6b7be8b98247f03f9175edc723024a0e9cf01f3c6/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4157532d53332d666639393030)](https://camo.githubusercontent.com/c36b22f42553605bb62b3dd6b7be8b98247f03f9175edc723024a0e9cf01f3c6/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4157532d53332d666639393030) [![Docker](https://camo.githubusercontent.com/2961351bf5692e9f5dcd03cf778bcd97ec3236dadeb35c763c213f4b152ec9a2/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f446f636b65722d436f6e7461696e6572697a65642d626c7565)](https://camo.githubusercontent.com/2961351bf5692e9f5dcd03cf778bcd97ec3236dadeb35c763c213f4b152ec9a2/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f446f636b65722d436f6e7461696e6572697a65642d626c7565)

---

## 🧾Project Overview

The system uses a **hybrid deep learning model (ANN + LSTM)** to analyze:

* user profile data (*age, weight, body fat, blood pressure*)
* daily activity data (*steps, active minutes, calories*)

**Based on this analysis, the system can:**

* predict fitness level
* estimate calorie burn
* generate personalized exercise recommendations
* provide 3D workout visualization
* track user fitness progress

## 💡Key Features

### 1️⃣ Health Prediction (ANN + LSTM)

The hybrid model analyzes both:

* static health features
* time-series activity patterns

to predict the user's  **fitness class or health condition** .

---

### 2️⃣ Calorie Burn Estimation

The system estimates the number of calories burned based on:

* daily steps
* activity intensity
* user body metrics

---

### 3️⃣ Personalized Workout Generator

Based on the predicted fitness level, the system generates:

* daily workout plans
* recommended activity goals
* exercise intensity suggestions

---

### 4️⃣ 3D Exercise Visualization

The platform provides **interactive 3D exercise demonstrations** to guide users in performing workouts correctly.

Technologies used may include:

* **Three.js**
* **Blender**

---

### 5️⃣ Camera-Based Posture Detection

Using computer vision, the system detects exercise posture and provides real-time feedback to improve workout form.

Possible tools:

* **MediaPipe**
* **OpenPose**

---

### 6️⃣ Progress Tracking Dashboard

Users can track:

* daily steps
* calories burned
* activity levels
* fitness score trends

---

## 🚀Model Architecture

![1773260707788](image/README/1773260707788.png)

---

## 🧠Technology Stack

#### Data Collection

The system uses a dataset that includes:

**-Activity Data.**

**-Health Profile Data.**

#### Data Preprocessing

Before training the model, the dataset undergoes preprocessing steps.Hybrid Model Architecture

##### Machine Learning/Deep Learnig

###### ANN & LSTM

**ANN**-Static user information.

**LSTM**-Time-series patterns.

* TensorFlow / Keras
* Scikit-learn
* Pandas

#### Model Training

The model is trained using:

* **TensorFlow / Keras**
* **Adam optimizer**
* **Sparse categorical crossentropy loss**

**MLOps**

* **DVC** for dataset versioning
* **MLflow** for experiment tracking

**Backend**

* FastAPI

**Frontend**

* React

**Deployment**

* Docker
* Kubernetes

**Cloud Storage**

* Amazon S3 Bucket

---

## 💎Project Pipeline

![1773260642259](image/README/1773260642259.png)

---



## ⚙️Tech Stack

| Category              | Technology                                                  | Purpose                                           |
| --------------------- | ----------------------------------------------------------- | ------------------------------------------------- |
| AI / Machine Learning | **TensorFlow**,**Keras**,**Scikit-learn** | Build and train ANN + LSTM models                 |
| Data Processing       | **Pandas**,**NumPy**                            | Data cleaning, preprocessing, feature engineering |
| Backend               | **FastAPI**,**Uvicorn**                         | API development and model serving                 |
| Frontend              | **React**,**Next.js**                           | User interface and dashboard                      |
| Computer Vision       | **MediaPipe**,**OpenCV**                        | Exercise posture detection                        |
| 3D Visualization      | **Three.js**,**Blender**                        | 3D exercise demonstration                         |
| MLOps                 | **DVC**,**MLflow**                              | Data versioning and experiment tracking           |
| Cloud Storage         | **Amazon S3**                                         | Store datasets and trained models                 |
| Deployment            | **Docker**,**Kubernetes**                       | Containerization and scalable deployment          |

---

## 🧰SmartFitness-AI Project Architecture

![1773260525283](image/README/1773260525283.png)

![1773260550305](image/README/1773260550305.png)
