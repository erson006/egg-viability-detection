# 🥚 Egg Viability Detection System

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

## 🏠 Main Menu

The main dashboard provides quick access to all application modules.

![Main Menu](images/mobile-home.png)

---

## 🎛️ Control Center

The Control Center is the core of the application. It connects to the ESP32-CAM, loads the TensorFlow Lite model, displays the live camera stream, and manages the image acquisition process.

![Control Center](images/control-center.png)

---

## 🌐 ESP32 Connection Settings

Users can configure the ESP32-CAM IP address directly from the application, allowing quick connection to different devices.

![ESP32 Settings](images/ip-settings.png)

---

## 💡 LED & 360° Stepper Motor Control

The application allows users to adjust LED brightness and control the 360° stepper motor for automated multi-angle image acquisition.

![LED & Stepper Motor](images/led-stepper-control.png)

---

## 🖼️ Smart Gallery

Captured images are automatically categorized and stored inside the application for easy access and review.

![Gallery](images/gallery.png)

---

## 📝 Automatic File Naming

To simplify dataset management, every captured image is automatically assigned a unique filename.

The filename contains:

- Image name
- Stepper motor angle
- Incremental index

This prevents duplicate filenames while preserving the capture position of every image.

![Automatic File Naming](images/file-naming.png)
