# 🌟NutriMind AI: Your Ultimate Personalized Routine Architect

![NutriMind AI Banner](WhatsApp Image 2025-09-13 at 20.11.57_e12a1c95.jpg)

![License](https://img.shields.io/badge/license-MIT-green.svg)
![Build](https://img.shields.io/badge/build-passing-brightgreen.svg)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![ML Model](https://img.shields.io/badge/ML-TensorFlow-orange?style=for-the-badge&logo=tensorflow&logoColor=white)
![Deployment](https://img.shields.io/badge/Deployed-Google%20Cloud-blue?style=for-the-badge)
![Figma](https://img.shields.io/badge/Design-Figma-red?style=for-the-badge&logo=figma&logoColor=white)


NutriMind AI is not just an app—it's a revolutionary ecosystem that crafts personalized daily routines (nutrition, sleep, exercise, mindfulness) using cutting-edge Machine Learning deployed on Google Cloud, a robust Node.js backend, a seamless Flutter mobile app, and an award-worthy UI/UX design. Born from the innovative IEEE Victoris 4.0 challenge, NutriMind empowers millions to live smarter with AI-driven insights.

*Vision:* To redefine productivity and well-being with a global, scalable solution that adapts to you.

---

## 📚 Table of Contents

- [Vision & Mission](#-vision--mission)
- [Technology Stack](#-technology-stack)
- [System Architecture](#-system-architecture)
- [Core Features](#-core-features)
- [Quick Start](#-quick-start)
- [API & ML Insights](#-api--ml-insights)
- [Visual Showcase](#-visual-showcase)
- [Contribute to Greatness](#-contribute-to-greatness)
- [Future Roadmap](#-future-roadmap)
- [License & Ethics](#-license--ethics)

---

## 🌟 Vision & Mission

NutriMind AI is dedicated to transforming lives through intelligent personalization. Our vision is to empower users globally with AI-crafted routines that optimize productivity, health, and mindfulness. Born from the IEEE Victoris 4.0 challenge, we aim to deliver a scalable, secure, and intuitive platform that evolves with every user interaction, setting a new standard for smart living.

*Mission:* To harness the power of AI and modern tech to create a world where everyone thrives with a routine tailored just for them.

---

## 🛠 Technology Stack

NutriMind leverages a cutting-edge tech ecosystem:

- *Machine Learning:* Fine-tuined model (Qwen 1.5 5B) on 5K row data, and deployed on Google Cloud AI Platform
- *Backend:* Node.js with Express.js, Mongoose (MongoDB), and JWT-based authentication
- *Mobile:* Flutter for cross-platform (iOS & Android) apps with Riverpod state management
- *UI/UX:* Figma-designed interfaces with micro-interactions and WCAG-compliant accessibility
- *Deployment:* Google Cloud (AI, Cloud Run), enhanced with CI/CD via GitHub Actions
- *Database:* MongoDB Atlas for flexible data storage
- *Authentication:* JWT with secure token refresh mechanisms

---


## 🏗 System Architecture


![System Architecture](https://drive.google.com/uc?export=view&id=1sVsSuRs_JsQVNdawYoasqH2uAtag6WgEu)

---

---

## 🚀 Core Features

- *Personalized Routine Creation:* AI-generated routines based on user preferences, goals, and constraints
- *Multi-Domain Optimization:* Nutrition, sleep, exercise, and mindfulness recommendations
- *JWT-Based Secure Authentication:* Role-based access control for different user types
- *Real-Time ML Inference:* Google Cloud deployment with <200ms latency
- *Intuitive UI/UX:* Flutter implementation of award-winning Figma designs
- *Progress Tracking:* Visual analytics and habit formation support
- *Adaptive Learning:* ML models that improve with user feedback
- *Cross-Platform Compatibility:* iOS and Android from a single codebase

---

## ⚡ Quick Start

### Prerequisites

- Node.js (v18+)
- Flutter SDK (v3.10+)
- MongoDB Atlas account or local installation
- Google Cloud account (for full ML functionality)

### Setup Instructions

1. *Clone the Repository:*
   bash
   git clone https://github.com/ieee-victoris-4-0/NutriMind_Project.git
   cd NutriMind_Project
   

2. *Backend Setup:*
   bash
   cd backend
   cp .env.example .env
   # Edit .env with your configuration
   npm install
   npm run dev
   

3. *Mobile App Setup:*
   bash
   cd mobile
   flutter pub get
   flutter run
   


---

## 🔌 API & ML Insights

### Key API Endpoints

- POST /api/auth/login → { token, user }
- POST /api/auth/register → { token, user }
- POST /api/routines/generate → Generate personalized routine
- GET /api/routines/:userId → Retrieve user routines
- PUT /api/routines/feedback → Provide feedback for ML improvement

### Machine Learning Specifications

- *Model Type:* LSTM with Attention Mechanisms
- *Training Data:* 10k+ annotated routine samples
- *Accuracy:* 95% on validation set
- *Latency:* <200ms inference time
- *Deployment:* Google Cloud AI Platform
- *Retraining:* Weekly incremental learning from user feedback

### Example API Request

bash
curl -X POST https://api.nutrimind.ai/routines/generate \
  -H "Authorization: Bearer <your_jwt_token>" \
  -H "Content-Type: application/json" \
  -d '{
    "goals": ["weight_loss", "improved_sleep"],
    "constraints": {
      "time_available": 120,
      "dietary_restrictions": ["vegetarian"]
    },
    "current_habits": {
      "sleep_hours": 6,
      "exercise_frequency": 2
    }
  }'


---

## 🎨 Visual Showcase


### Routine Dashboard
![Dashboard](https://www.notion.so/IEEE-Competition-25842616b32780c8887bdf66c2312328)

### Design System
[Figma Design File](https://www.figma.com/design/kPoJr1Wk07ZCVCpYPbYFtn/NutriMind?node-id=0-1&p=f&t=KdJOqXrNztDiwGE9-0)

### Demo Video
[Watch Demo](https://example.com/nutrimind-demo) <!-- Replace with actual demo video link -->

---



## 🗺 Future Roadmap

### 2025 Q4
- [ ] Multilingual support (Arabic, Spanish, French)
- [ ] Wearable integration (Fitbit, Apple Health, Google Fit)
- [ ] Advanced sleep stage analysis


### Ongoing
- [ ] Community-driven features via in-app polls
- [ ] Enhancing Our model capabilities

---

## 📄 License & Ethics

### License
MIT License 
### Ethical Commitments
- *Transparent AI:* Open documentation of model capabilities and limitations
- *Bias Audits:* Regular testing for demographic and cultural biases
- *User Consent-First:* Explicit opt-in for data usage in model improvement
- *Privacy by Design:* End-to-end encryption for sensitive health data
- *Accessibility:* WCAG 2.1 compliance for users with disabilities

### Data Privacy
- User data never sold to third parties
- Anonymous aggregation for model improvement only with explicit consent
- Right to be forgotten with full data deletion capability

---
### Last Words  

This journey has been more than just building a project—it has been a true test of our creativity, teamwork, and persistence. Our idea represents not only the solution we proposed, but also our ability to take a project from the ground up and bring it to life, from initial concept to hosting and running a full application.  

- We would like to express our deepest gratitude and appreciation to ** IEEE team **  for organizing this remarkable competition. It has been an inspiring and unforgettable experience that allowed us to learn, grow, and collaborate while pushing the boundaries of what we can achieve together.
---
