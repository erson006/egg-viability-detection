# 🥚 Egg Viability Detection System

<p align="center">

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)

![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)

![TensorFlow Lite](https://img.shields.io/badge/TensorFlow_Lite-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)

![Edge Impulse](https://img.shields.io/badge/Edge_Impulse-4B6BFB?style=for-the-badge)

![ESP32-CAM](https://img.shields.io/badge/ESP32--CAM-00979D?style=for-the-badge)

![Computer Vision](https://img.shields.io/badge/Computer_Vision-AI-success?style=for-the-badge)

</p>

## 📑 Table of Contents

- [Project Overview](#-project-overview)
- [Core Features](#-core-features)
- [Mobile Application](#-mobile-application)
- [AI Model Performance](#-ai-model-performance)
- [System Architecture](#-system-architecture)
- [Technologies Used](#️-technologies-used)
- [Source Code Availability](#-source-code-availability)
- [Future Improvements](#-future-improvements)

An AI-powered egg viability detection system developed using **Flutter**, **ESP32-CAM**, **TensorFlow Lite**, and **Edge Impulse**.

This project captures egg images through an ESP32-CAM module and performs local AI inference using a TensorFlow Lite model inside the Flutter mobile application.

The application also provides camera management, LED brightness control, 360° stepper motor control, image gallery management, and automated image capture for egg inspection.

> **Note:** This repository showcases the project architecture, mobile application, and AI performance. The complete source code, trained models, and datasets are maintained in a private repository.

---

# ✨ Core Features

## 🤖 Artificial Intelligence

- Egg viability classification using TensorFlow Lite
- Edge Impulse transfer learning model
- 99%+ validation accuracy
- Local AI inference on the mobile device
- Confusion Matrix
- Precision, Recall and F1 Score evaluation

## 📱 Mobile Application

- Live ESP32-CAM stream
- Prediction interface
- Smart gallery
- ESP32 IP configuration

## ⚙️ Embedded Hardware

- ESP32-CAM
- Adjustable LED brightness
- 360° stepper motor control
- Single image capture
- Multi-angle image capture

## 📂 Dataset Management

- Automatic filename indexing
- Servo angle added to image filename
- Categorized gallery
- Automatic image organization

---

# 📱 Mobile Application

The Flutter mobile application is responsible for controlling the hardware, managing image acquisition, and performing on-device AI inference using a TensorFlow Lite (Float32) model.

<table>
<tr>
<td align="center">
<b>🏠 Main Menu</b><br><br>
<img src="images/mobile-home.png" width="220">
</td>

<td align="center">
<b>🎛️ Control Center</b><br><br>
<img src="images/control-center.png" width="220">
</td>

<td align="center">
<b>🌐 ESP32 Settings</b><br><br>
<img src="images/ip-settings.png" width="220">
</td>
</tr>

<tr>
<td align="center">
<b>💡 LED & 360° Stepper Motor</b><br><br>
<img src="images/led-stepper-control.png" width="220">
</td>

<td align="center">
<b>🖼️ Smart Gallery</b><br><br>
<img src="images/gallery.png" width="220">
</td>

<td align="center">
<b>📝 Automatic File Naming</b><br><br>
<img src="images/file-naming.png" width="220">
</td>
</tr>
</table>

### ✨ Key Capabilities

- 📷 Live camera stream from ESP32-CAM
- 🧠 Local AI inference using TensorFlow Lite (Float32)
- 💡 Adjustable LED brightness
- ⚙️ 360° stepper motor control
- 📸 Single and multi-angle image capture
- 🗂️ Smart gallery with categorized images
- 📝 Automatic file naming with angle metadata and incremental indexing

# 🧠 AI Model Performance

The egg viability classification model was trained using **Edge Impulse** with **Transfer Learning** and deployed as a **TensorFlow Lite (Float32)** model for on-device inference in the Flutter application.

The model achieves high classification performance while running entirely on the mobile device without requiring an internet connection.

---

## 📊 Transfer Learning Results

The following metrics summarize the performance of the trained model.

- Accuracy
- Loss
- Precision
- Recall
- F1 Score
- ROC AUC
- Confusion Matrix

![Transfer Learning Results](images/transfer-learning-results.png)

---

## ✅ Model Testing Results

The trained TensorFlow Lite model was evaluated using unseen test images to verify its real-world performance.

![Model Testing Results](images/model-testing-results.png)

---

## 📈 Feature Explorer

The Feature Explorer visualization demonstrates how the extracted image features are grouped by the trained model. A clear separation between classes indicates strong feature learning and improved classification capability.

![Feature Explorer](images/feature-explorer.png)

---

## 📉 Data Explorer

The Data Explorer provides an overview of the labeled dataset used during training and helps verify the quality and distribution of collected samples.

![Data Explorer](images/data-explorer.png)

## 🏗️ System Architecture

```mermaid
flowchart TD

A([🥚 Egg])

B[📷 ESP32-CAM<br/>Live Camera Stream]

C[📱 Flutter Mobile Application]

D[🧠 TensorFlow Lite<br/>Float32]

E{Prediction}

F[🟢 Fertilized Egg]

G[⚪ Unfertilized Egg]

H[💡 LED Brightness Control]

I[⚙️ 360° Stepper Motor]

J[📸 Image Capture]

K[📂 Smart Gallery]

L[📝 Automatic File Naming]

M[📐 Stepper Angle Metadata]

N[#️⃣ Incremental Index]

A --> B

B -->|Wi-Fi| C

C --> D

D --> E

E --> F

E --> G

C --> H

C --> I

C --> J

J --> K

K --> L

L --> M

M --> N
```

---

# 🛠️ Technologies Used

| Category | Technology |
|----------|------------|
| Mobile Framework | Flutter |
| Programming Language | Dart |
| AI Framework | TensorFlow Lite (Float32) |
| AI Development Platform | Edge Impulse |
| Embedded Hardware | ESP32-CAM |
| Motor Control | 360° Stepper Motor |
| Lighting System | Adjustable LED |
| Communication | Wi-Fi |
| Machine Learning | Transfer Learning |
| Computer Vision | Image Classification |

---

# 🔒 Source Code Availability

This repository showcases the project's architecture, methodology, mobile application, and AI model performance.

The complete source code, TensorFlow Lite model, Edge Impulse project, datasets, and embedded firmware are kept in a private repository to protect the project's intellectual property.

If you are interested in collaboration, research, commercial licensing, or a live demonstration, please feel free to contact me.


