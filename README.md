# CropSense AI 🌱
### Intelligent Crop Recommendation System Powered by Machine Learning

<p align="center">
  A production-ready full-stack AI application that recommends the most suitable crop based on soil composition and environmental conditions.
</p>

---

## 🚀 Live Demo

- 🌐 Frontend: https://cropsense-crop-recommendation.vercel.app
- 🔗 API Health Check: https://cropsense-api-wjbv.onrender.com/api/health

---

# 📌 Overview

CropSense AI is a modern full-stack machine learning platform designed to assist farmers, researchers, and agricultural professionals in selecting the most suitable crop based on soil nutrients and environmental conditions.

The application uses a trained **Random Forest Machine Learning model** developed with **Scikit-learn** to analyze agricultural parameters and generate accurate crop recommendations in real time.

The platform combines:

- 🤖 Machine Learning Intelligence
- ⚡ High-Performance Backend APIs
- 🎨 Modern Responsive Frontend UI
- ☁️ Cloud-Based Deployment Architecture

This project demonstrates the integration of Artificial Intelligence with modern web technologies to build practical agricultural solutions.

---

# ✨ Key Features

## 🤖 AI-Powered Crop Recommendation

- Uses a Random Forest Machine Learning model
- High-accuracy crop prediction system
- Real-time recommendation generation
- Supports prediction for 22 crop categories

---

## 🎨 Modern UI/UX Design

- Premium glassmorphism interface
- Dark-theme inspired design
- Smooth responsive layouts
- Modern component architecture

---

## 📱 Fully Responsive

Optimized for:

- Desktop Computers
- Tablets / iPads
- Smartphones

---

## 🔒 Secure & Production-Ready

- Environment variable protection
- Secure CORS configuration
- Input validation & sanitization
- Decoupled frontend/backend architecture

---

## ☁️ Cloud Deployment

- Frontend deployed on Vercel
- Backend deployed on Render
- Scalable REST API architecture

---

# 🧠 Machine Learning Overview

The recommendation engine is powered by a **Random Forest Classifier** trained on agricultural datasets containing more than **2,200 records**.

The system predicts the most suitable crop based on multiple environmental and soil parameters.

---

## 📊 Input Parameters

| Parameter | Description |
|---|---|
| Nitrogen (N) | Nitrogen content in soil |
| Phosphorus (P) | Phosphorus content in soil |
| Potassium (K) | Potassium content in soil |
| Temperature | Temperature in Celsius |
| Humidity | Relative humidity percentage |
| pH | Soil pH value |
| Rainfall | Rainfall amount in mm |

---

## 🌾 Supported Crops

The model supports prediction for multiple crop categories including:

- Rice
- Wheat
- Maize
- Cotton
- Mango
- Banana
- Apple
- Coconut
- Coffee
- Chickpea
- Kidney Beans
- Lentils
- Pomegranate
- Watermelon
- Orange
- Papaya
- Jute
- Grapes
- Blackgram
- Muskmelon
- Pigeon Peas
- Moth Beans

---

# 🛠️ Tech Stack

## Frontend

- React 18
- Vite
- CSS Modules
- Lucide React Icons

---

## Backend

- Node.js
- Express.js
- Python 3

---

## Machine Learning

- Scikit-learn
- NumPy
- Pickle

---

## Deployment Platforms

- Vercel (Frontend)
- Render (Backend)

---

# 🏗️ System Architecture

```text
Frontend (React)
       ↓
REST API (Express.js)
       ↓
Python ML Prediction Script
       ↓
Random Forest ML Model
       ↓
Prediction Response
```

---

# 📂 Project Structure

```bash
Crop_Recomendation/
│
├── cap_backend/                     # Express + Python Backend
│   ├── server.js                    # Express server entry point
│   ├── predict.py                   # Python ML prediction bridge
│   ├── requirements.txt             # Python dependencies
│   ├── model_files/                 # Trained ML models & scalers
│   ├── routes/                      # API route handlers
│   └── .env                         # Backend environment variables
│
├── cap_frontend/                    # React Frontend
│   ├── src/
│   │   ├── pages/                   # Application pages
│   │   ├── components/              # Reusable components
│   │   ├── services/                # API services
│   │   └── index.css                # Global styling
│   │
│   ├── public/
│   ├── vercel.json                  # Vercel deployment configuration
│   └── .env                         # Frontend environment variables
│
├── screenshots/                     # Project screenshots
├── README.md
└── .gitignore
```

---

# ⚙️ Local Development Setup

## 📋 Prerequisites

Ensure the following are installed:

- Node.js v18 or higher
- Python 3.10 or higher
- npm or yarn
- Git

---

# 🔧 Backend Setup

## Step 1 — Navigate to Backend Folder

```bash
cd cap_backend
```

---

## Step 2 — Install Dependencies

```bash
npm install
pip install -r requirements.txt
```

---

## Step 3 — Start Backend Server

```bash
npm start
```

Backend server runs on:

```bash
http://localhost:5002
```

---

# 💻 Frontend Setup

## Step 1 — Navigate to Frontend Folder

```bash
cd cap_frontend
```

---

## Step 2 — Install Dependencies

```bash
npm install
```

---

## Step 3 — Start Development Server

```bash
npm run dev
```

Frontend runs on:

```bash
http://localhost:5173
```

---

# 🌐 API Documentation

# Health Check Endpoint

## Request

```http
GET /api/health
```

---

## Response

```json
{
  "status": "ok",
  "message": "Crop Recommendation API is running"
}
```

---

# Crop Prediction Endpoint

## Request

```http
POST /api/predict
```

---

## Sample Request Body

```json
{
  "N": 90,
  "P": 42,
  "K": 43,
  "temperature": 20.8,
  "humidity": 82,
  "ph": 6.5,
  "rainfall": 202.9
}
```

---

## Sample Response

```json
{
  "prediction": "rice"
}
```

---

# ☁️ Deployment Architecture

The project follows a modern dual-platform cloud deployment strategy.

---

## 🌐 Frontend Deployment

### Platform: Vercel

Features:

- Fast global CDN delivery
- Optimized Vite production build
- SPA routing support
- Automatic GitHub deployment

---

## ⚙️ Backend Deployment

### Platform: Render

Features:

- Native Node.js + Python support
- Machine Learning model hosting
- REST API deployment
- Environment variable management

---

# 🔐 Environment Variables

## Backend `.env`

```env
PORT=5002
FRONTEND_URL=http://localhost:5173
```

---

## Frontend `.env`

```env
VITE_API_URL=http://localhost:5002/api
```

---

# 📸 Screenshots

## Landing Page

Add screenshot here

---

## Prediction Interface

Add screenshot here

---

## Mobile Responsive Design

Add screenshot here

---

# 📈 Future Enhancements

Planned future improvements include:

- 🌦 Real-time Weather API Integration
- 🛰 Soil Analysis Integration
- 📊 Agricultural Analytics Dashboard
- 📱 Mobile Application
- 🌍 Multi-language Support
- 🧠 Deep Learning-Based Prediction
- 📈 Crop Yield Estimation
- ☁️ Cloud Database Integration

---

# 🧪 Testing & Validation

The application includes:

- Backend validation middleware
- API error handling
- Prediction verification
- Responsive UI testing
- Cross-device compatibility checks

---

# 📄 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

## Kaif Islam

Full Stack Developer • Machine Learning Enthusiast • AI Application Developer

---

# ⭐ Acknowledgements

Special thanks to:

- Scikit-learn
- React Community
- Vercel
- Render
- Open Source ML Datasets

---

# 📬 Feedback & Contributions

Contributions, suggestions, and feedback are always welcome.

If you found this project useful, consider giving it a ⭐ on GitHub.