# 🏭 Industrial Defect Detection System

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![Python](https://img.shields.io/badge/python-3.9+-green.svg)
![React](https://img.shields.io/badge/react-18.0+-cyan.svg)
![License](https://img.shields.io/badge/license-MIT-yellow.svg)

> A comprehensive computer vision system for real-time industrial defect detection with edge deployment capabilities.

## 📋 Table of Contents
- [Overview](#-overview)
- [Features](#-features)
- [Architecture](#-architecture)
- [Tech Stack](#-tech-stack)
- [Installation](#-installation)
- [Usage](#-usage)
- [API Documentation](#-api-documentation)
- [Model Details](#-model-details)
- [Performance](#-performance)
- [Project Structure](#-project-structure)
- [Contributing](#-contributing)
- [License](#-license)

## 🎯 Overview

The **Industrial Defect Detection System** is a production-ready computer vision solution designed for manufacturing quality control. It leverages state-of-the-art deep learning models (YOLOv8, ResNet, EfficientNet) to detect defects in industrial products in real-time.

### Problem Statement
Manufacturing defects cost industries billions annually. Traditional manual inspection is:
- ❌ Slow and labor-intensive
- ❌ Prone to human error
- ❌ Inconsistent results
- ❌ High operational costs

### Our Solution
This system provides:
- ✅ Automated 24/7 defect detection
- ✅ High accuracy with multiple models
- ✅ Real-time processing
- ✅ Edge deployment for cost savings
- ✅ Model compression for efficiency
- ✅ AI-powered analysis with Gemini

## ✨ Features

### Core Features
- **🔍 Multi-Model Support**: YOLOv8, ResNet50, EfficientNet
- **⚡ Real-Time Detection**: Process images in milliseconds
- **📊 Performance Benchmarking**: Track accuracy, speed, resource usage
- **🗜️ Model Compression**: Pruning, quantization, knowledge distillation
- **🌐 Edge Deployment**: CPU-optimized inference
- **🤖 Gemini Integration**: AI analysis and defect description
- **📈 Interactive Dashboard**: Visual analytics and charts
- **🎨 Modern UI**: Responsive, dark/light mode
- **📱 Mobile Ready**: Works on all devices

### Advanced Features
- **Batch Processing**: Process multiple images
- **History Tracking**: View past detections
- **Export Results**: Generate reports (PDF/CSV)
- **Model Comparison**: Compare models side-by-side
- **Real-time Metrics**: FPS, latency, accuracy
- **Defect Classification**: Multi-class detection

## 🏗️ Architecture

echo " " >> README.md
echo "## 📅 Last Updated: $(Get-Date)" >> README.md


## 🛠️ Tech Stack

### Backend
| Technology | Version | Purpose |
|------------|---------|---------|
| Python | 3.9+ | Core programming language |
| Flask/FastAPI | Latest | REST API framework |
| YOLOv8 | 8.0+ | Object detection |
| PyTorch | 2.0+ | Deep learning framework |
| OpenCV | 4.8+ | Image processing |
| SQLAlchemy | 2.0+ | ORM for database |
| Scikit-learn | 1.3+ | Metrics calculation |

### Frontend
| Technology | Version | Purpose |
|------------|---------|---------|
| React | 18.0+ | UI framework |
| Vite | 4.0+ | Build tool |
| Tailwind CSS | 3.0+ | Styling framework |
| Chart.js | 4.0+ | Data visualization |
| Axios | 1.5+ | HTTP client |
| React Router | 6.0+ | Routing |

### Database
| Technology | Purpose |
|------------|---------|
| SQLite | Development database |
| PostgreSQL | Production database |

### Additional Tools
- **Docker**: Containerization
- **Git**: Version control
- **Gemini API**: AI integration
- **Pytest**: Testing
- **Loguru**: Logging

## 📦 Installation

### Prerequisites
- Python 3.9+
- Node.js 16+
- npm or yarn
- Git

### Step 1: Clone Repository
```bash
git clone https://github.com/yourusername/Industrial-Defect-Detection-System.git
cd Industrial-Defect-Detection-System

# Create virtual environment
cd backend
python -m venv venv

# Activate virtual environment
# Windows
venv\Scripts\activate
# Mac/Linux
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Create .env file
cp .env.example .env
# Edit .env with your configurations

# Initialize database
python -c "from app.models.database import init_db; init_db()"

# Run backend server
python run.py

# Open new terminal
cd frontend

# Install dependencies
npm install

# Create .env file
cp .env.example .env
# Edit .env with backend URL

# Run frontend development server
npm run dev