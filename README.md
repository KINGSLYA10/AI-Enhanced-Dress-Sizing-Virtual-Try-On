# AI-Enhanced-Dress-Sizing-Virtual-Try-On

An AI-powered solution that solves the online clothing "fit problem" by using computer vision to take accurate body measurements through a webcam, recommending the right size, and letting users try on clothes virtually via a privacy-preserving 3D avatar — without ever exposing their real face or body.

---

## 📌 Problem Statement

Online shopping in India is booming — **185M+ annual shoppers in 2021**, projected to reach **425M by 2027** — and clothing is the single most purchased *and* most returned category (47%+ of returns). The core reason: customers can't be sure of their size without physically trying the garment on.

This project builds an AI mechanism that replaces the "tailor at home" experience with a camera-based measurement and virtual try-on system, while keeping user privacy front and center.

## 🎯 Objectives

- Accurately measure body dimensions (shoulder, waist, hand, etc.) using a camera-based, ML/pose-estimation approach — for both men and women.
- Recommend the correct clothing size (S/M/L/XL/XXL) based on real measurements.
- Protect user privacy by generating a digital **avatar** instead of storing/exposing raw face or body images.
- Enforce AI safety restrictions that prevent inappropriate/undressing behavior.
- Provide a **virtual try-on** experience so users can preview garments before purchase.
- Offer **style recommendations** based on body shape, personal taste, and current fashion trends.

## ✨ Key Features

| Feature | Description |
|---|---|
| 📷 Camera-Based Measurement | Uses pose estimation to extract shoulder, waist, and hand measurements in real time |
| 🧠 AI Size Prediction | ML model maps measurements to standard sizes (S, M, L, XL, XXL) |
| 🕶️ Privacy-First Avatar | Generates a 3D avatar from measurements so real face/body images are never exposed or stored |
| 🚫 Safety Guardrails | Built-in restrictions preventing undressing/inappropriate AI outputs |
| 👗 Virtual Try-On | Overlays selected garments onto the user's avatar with a 360° view |
| 🎨 Style Recommendations | Suggests outfits/combinations based on body shape and fashion trends |
| 🛒 E-commerce Style UI | Familiar shopping flow — login via OTP, browse, select size/color, try on, checkout |

## 🏗️ System Architecture

The prototype is built around four core modules:

1. **Module I — User Side Interface**
   Responsive UI for browsing products and logging in securely via OTP (email/mobile).

2. **Module II — Measuring Unit**
   Activates the AI camera to capture and compute body measurements (shoulder, hand, waist) and predicts the recommended size.

3. **Module III — Virtual Try-On Unit**
   Overlays the selected garment on the live camera feed and evaluates fit (tightness, looseness, length) against the user's skin tone, hair type, and body type using computer vision.

4. **Module IV — Avatar Unit**
   Uses AR to render the garment on a customizable 3D avatar (360° view), with options to add accessories (watch, chain, cap, earrings) and footwear (shoes, slippers).

```
User Interface  →  Measuring Unit  →  Virtual Try-On Unit  →  Avatar Unit
   (Login/UI)      (Pose + Size)      (Fit Evaluation)       (AR Preview)
```

## 🛠️ Tech Stack

**Hardware**
- Basic Camera
- Laptop with GPU (Graphics Processing Unit)
- Storage Device

**Software**
- Windows OS
- Python 3.7.0
- Visual Studio Code
- MySQL
- OpenCV, MediaPipe (Image Processing)
- Pose Estimation Libraries
- GitHub (Version Control)

## 🚀 Getting Started

### Prerequisites
- Python 3.7+
- MySQL Server
- A working webcam
- (Recommended) A CUDA-capable GPU for faster pose estimation

### Installation
```bash
# Clone the repository
git clone https://github.com/<your-username>/ai-dress-sizing-system.git
cd ai-dress-sizing-system

# Create and activate a virtual environment (optional but recommended)
python -m venv venv
venv\Scripts\activate   # Windows

# Install dependencies
pip install -r requirements.txt
```

### Running the App
```bash
python app.py
```
Then open the app in your browser/UI client, log in via OTP, select a product, and click **Virtual Try-On** to start the camera-based measurement flow.

## 📊 Market Insights (Why This Matters)

- Clothing is the **#1** most-purchased (51%) and **#1** most-returned (47%+) category in Indian e-commerce.
- India's e-commerce market is projected to hit **US$199.2B by 2028** (17.4% CAGR).
- Reducing size-related returns directly improves customer satisfaction and reduces logistics/reverse-shipping costs for retailers.

## 🔒 Privacy & Safety by Design

- Real face/body footage is used only transiently to compute measurements and generate an avatar — it is **not** used for display or storage.
- Explicit AI restrictions are built in to prevent misuse or generation of inappropriate imagery.
- All personalization (try-on, style recommendations) happens on the anonymized avatar, not the user's real image.

## 📈 Future Scope

- Expand measurement accuracy across more body types and clothing categories (footwear, accessories).
- Integrate deep learning-based fit scoring for more nuanced recommendations.
- Add multi-angle camera support for improved 3D avatar fidelity.
- Deploy as a browser extension / mobile app for wider e-commerce integration.

## 👥 Team

| Name | Register No. | Year |
|---|---|---|
| A. Kingsly | 211422243159 | II Year AIDS |
| V. Jeeva | 211422243118 | II Year AIDS |
| H. Lionel Vasantha Raj | 211422243177 | II Year AIDS |
| R. S. Kishore | 211422243167 | II Year AIDS |

**Mentor:** Mrs. S. Hemamalini, M.E., Associate Professor, Department of Artificial Intelligence and Data Science

**Institution:** Panimalar Engineering College, Chennai – 600 123
Department of Artificial Intelligence and Data Science

## 📄 License

This project was developed as an academic project. Add a license (e.g., MIT) here if you plan to open-source it.
