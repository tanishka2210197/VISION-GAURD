# 👁️ VisionGuard – Real-Time Pedestrian Video Anomaly Detection System

## 📌 Overview

**VisionGuard** is a **real-time video anomaly detection system** designed to identify unusual pedestrian activities in surveillance footage.

The system leverages a **Hybrid Model combining spatial and temporal learning** to detect anomalies such as suspicious movement patterns, crowd irregularities, or unexpected behaviors in real-world environments.

---

## 🚀 Key Features

* 🎥 Real-time anomaly detection in video streams
* 🧠 Hybrid deep learning architecture (SDE + ConvLSTM)
* ⚡ Ultra-low latency (**< 25 ms/frame**)
* 📊 High performance (**~94% AUC**) across benchmark datasets
* 🔍 Explainable AI with saliency and attention heatmaps
* 🛡️ Designed for intelligent surveillance systems

---

## 🧠 Model Architecture

### 🔷 Hybrid HMSPN (Hybrid Multi-Stage Predictive Network)

The model integrates:

#### 1️⃣ Sparse Denoising Encoder (SDE)

* Learns **robust spatial representations**
* Removes noise and focuses on key visual features
* Helps in identifying structural anomalies

#### 2️⃣ ConvLSTM-based Temporal Frame Predictor

* Captures **temporal dependencies across frames**
* Predicts future frames based on past sequences
* Detects anomalies via **prediction error**

---

## ⚙️ Workflow

1. 🎞️ Input video frames
2. 🧹 Preprocessing & normalization
3. 🧠 Feature extraction using SDE
4. ⏳ Temporal modeling using ConvLSTM
5. 🔮 Frame prediction
6. ⚠️ Anomaly scoring based on reconstruction/prediction error
7. 📊 Visualization using attention & saliency maps

---

## 📊 Performance

| Metric    | Value             |
| --------- | ----------------- |
| AUC Score | **~94%**          |
| Latency   | **< 25 ms/frame** |
| Mode      | Real-time         |

---

## 📂 Datasets Used

* UCSD Ped1
* UCSD Ped2
* Avenue Dataset
* ShanghaiTech Dataset

These datasets include real-world surveillance scenarios with labeled anomalies.

---

## 🔍 Explainability Module

To enhance interpretability, VisionGuard includes:

* 🔥 Gradient-based saliency maps
* 🎯 Spatiotemporal attention maps

👉 These generate **heatmaps highlighting anomalous regions**, making the system suitable for real-world surveillance applications.

---

## 🛠️ Tech Stack

* **Programming Language:** Python
* **Frameworks & Libraries:**

  * PyTorch / TensorFlow
  * OpenCV
  * NumPy
  * Matplotlib

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/visionguard.git
cd visionguard
```

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the model

```bash
python main.py
```

---

## 📈 Applications

* 🏙️ Smart city surveillance
* 🚶 Pedestrian safety monitoring
* 🏢 Security in public spaces (airports, malls, stations)
* 🚨 Early detection of suspicious activities

---

## ⚠️ Challenges & Limitations

* Requires high-quality video input
* Performance may vary with extreme lighting/weather conditions
* Computationally intensive for large-scale deployment

---

## 🔮 Future Improvements

* 🤖 Integrate Transformer-based video models
* 🌐 Deploy as a real-time web dashboard
* 📱 Edge deployment for smart cameras
* 📊 Multi-class anomaly classification

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repo and submit a pull request.


⭐ If you find this project useful, please give it a **star**!
