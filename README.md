# 🤟 Eshara — Egyptian Sign Language Translator

> **Breaking communication barriers with AI 🇪🇬**

Eshara is an AI-powered Egyptian Sign Language (ESL) translator designed to help bridge the communication gap between people who use Egyptian Sign Language and people who do not understand it.

The system uses **Computer Vision** and **Deep Learning** to recognize Egyptian sign language gestures from camera input and convert them into **Arabic text and speech**.

---

## 🎯 Project Overview

Communication can be difficult between deaf and hearing people when they do not share the same language.

Most existing sign language recognition systems focus on **American Sign Language (ASL)** or recognize individual letters.

**Eshara focuses on Egyptian Sign Language** and aims to recognize useful everyday expressions and convert them into understandable Arabic text and voice.

### Example

```text
🤟 Sign Gesture
      ↓
📷 Camera
      ↓
👁️ Computer Vision
      ↓
🖐️ Hand / Pose Landmark Extraction
      ↓
🧠 Deep Learning Model
      ↓
📝 Arabic Text
      ↓
🔊 Speech
```

---

## 🚀 Main Features

* 🎥 Real-time camera-based sign recognition
* 🤟 Egyptian Sign Language recognition
* 🧠 Deep Learning-based classification
* 👁️ Computer Vision preprocessing
* 📝 Conversion of signs into Arabic text
* 🔊 Text-to-Speech output
* 🌐 Interactive web application
* 📊 Model evaluation and performance analysis

---

## 🧠 Technologies

| Technology           | Purpose                          |
| -------------------- | -------------------------------- |
| Python               | Main programming language        |
| OpenCV               | Image and video processing       |
| MediaPipe            | Hand and pose landmark detection |
| TensorFlow / PyTorch | Deep Learning                    |
| LSTM / Transformer   | Sign sequence classification     |
| Flask / FastAPI      | Backend API                      |
| Streamlit            | Web application                  |
| Git & GitHub         | Version control                  |

---

## 📊 Dataset

A custom Egyptian Sign Language dataset will be created for this project.

The dataset will contain videos representing common Egyptian sign language words and expressions.

### Planned Dataset

* Multiple Egyptian Sign Language classes
* Multiple videos per class
* Different users
* Different backgrounds and lighting conditions
* Training / validation / testing split

Example categories may include:

```text
Hello
Thank You
Help
Eat
Drink
Tired
Yes
No
Good
Bad
...
```

> The final dataset classes and number of samples will be updated after the data collection phase.

For privacy and repository size considerations, the complete raw video dataset will not be stored directly in this GitHub repository.

---

## 🏗️ System Architecture

```text
                ┌─────────────────┐
                │      Camera     │
                └────────┬────────┘
                         ↓
                ┌─────────────────┐
                │     OpenCV      │
                └────────┬────────┘
                         ↓
                ┌─────────────────┐
                │    MediaPipe    │
                │ Hand / Pose     │
                │   Landmarks     │
                └────────┬────────┘
                         ↓
                ┌─────────────────┐
                │ Deep Learning   │
                │ LSTM /          │
                │ Transformer     │
                └────────┬────────┘
                         ↓
                ┌─────────────────┐
                │ Sign Prediction │
                └────────┬────────┘
                         ↓
                ┌─────────────────┐
                │   Arabic Text   │
                └────────┬────────┘
                         ↓
```
