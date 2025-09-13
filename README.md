# 🌟 NutriMind AI: Your Ultimate Personalized Routine Architect

![NutriMind AI Banner](https://github.com/user-attachments/assets/530a7dcd-e01d-49ff-910b-ddcea430502f)

NutriMind AI is not just an app—it's a revolutionary ecosystem that crafts personalized daily routines (nutrition, sleep, exercise, mindfulness) using cutting-edge Machine Learning deployed on Google Cloud, a robust Node.js backend, a seamless Flutter mobile app, and an award-worthy UI/UX design. Born from the innovative IEEE Victoris 4.0 challenge, NutriMind empowers millions to live smarter with AI-driven insights.

**Vision:** To redefine productivity and well-being with a global, scalable solution that adapts to you.

![License](https://img.shields.io/badge/license-MIT-green.svg)
![Build](https://img.shields.io/badge/build-passing-brightgreen.svg)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![ML Model](https://img.shields.io/badge/ML-TensorFlow-orange?style=for-the-badge&logo=tensorflow&logoColor=white)
![Deployment](https://img.shields.io/badge/Deployed-Google%20Cloud-blue?style=for-the-badge)
![Figma](https://img.shields.io/badge/Design-Figma-red?style=for-the-badge&logo=figma&logoColor=white)

---

## 📚 Table of Contents

- [Vision & Mission](#-vision--mission)
- [Overview](#-overview)
- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)
- [System Architecture](#-system-architecture)
- [Core Features](#-core-features)
- [Quick Start](#-quick-start)
- [API & ML Insights](#-api--ml-insights)
- [Visual Showcase](#-visual-showcase)
- [Future Roadmap](#-future-roadmap)
- [License & Ethics](#-license--ethics)
- [Contributing](#-contributing)
- [Acknowledgments](#-acknowledgments)

---

## 🌟 Vision & Mission

NutriMind AI is dedicated to transforming lives through intelligent personalization. Our vision is to empower users globally with AI-crafted routines that optimize productivity, health, and mindfulness. Born from the IEEE Victoris 4.0 challenge, we aim to deliver a scalable, secure, and intuitive platform that evolves with every user interaction, setting a new standard for smart living.

**Mission:** To harness the power of AI and modern tech to create a world where everyone thrives with a routine tailored just for them.

---

## 🌟 Overview

NutriMind collects detailed health and lifestyle data via interactive surveys (name, DOB, weight, height, sleep patterns, fatigue levels, headache frequency, diet habits, activity level, etc.) and generates personalized daily routines split into Morning, Mid-day, Evening, and Night segments.

---

## ✨ Key Features

- 🎬 **Professional Onboarding**: Smooth user introduction experience
- ✅ **Authentication System**: Secure login with session persistence
- 📝 **Comprehensive Health Surveys**: Detailed data collection for tailored recommendations
- 🍏 **Personalized Daily Routines**: AI-generated task lists for optimal daily structure
- 💪 **Task Tracking System**: Simple completion tracking for daily tasks
- 🎨 **Modern UI/UX**: Beautiful interface with dark mode support
- ⚙️ **Efficient State Management**: flutter_bloc (Cubit) for optimal performance
- 🌐 **Seamless Backend Communication**: dio with cookie management integration

---

## 🛠 Tech Stack

| Layer | Technology |
|-------|------------|
| **Language** | Dart |
| **Framework** | Flutter |
| **State Management** | flutter_bloc (Cubit) |
| **Networking** | dio |
| **Cookie Management** | dio_cookie_manager, cookie_jar |
| **Icons** | font_awesome_flutter |
| **Fonts** | google_fonts |
| **Backend** | Node.js, Express.js |
| **Database** | MongoDB |
| **Authentication** | JWT |
| **ML Framework** | TensorFlow |
| **Deployment** | Google Cloud Platform |

---

## 🏗 System Architecture

![System Architecture](https://github.com/user-attachments/assets/229f002a-5d9e-405b-a3f1-010745b06885)

---

## 🚀 Core Features

- **Personalized Routine Creation**: AI-generated routines based on user preferences, goals, and constraints
- **Multi-Domain Optimization**: Nutrition, sleep, exercise, and mindfulness recommendations
- **JWT-Based Secure Authentication**: Role-based access control for different user types
- **Real-Time ML Inference**: Google Cloud deployment with <200ms latency
- **Intuitive UI/UX**: Flutter implementation of award-winning Figma designs
- **Progress Tracking**: Visual analytics and habit formation support
- **Adaptive Learning**: ML models that improve with user feedback
- **Cross-Platform Compatibility**: iOS and Android from a single codebase

---

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/Ahmed-S-A-A/NutriMind.git
cd NutriMind
```

### 2. Install Dependencies
```bash
flutter pub get
```

### 3. Run the Application
```bash
flutter run
```

### ⚠️ Important Notes Before Deployment
- Ensure all assets are properly declared in `pubspec.yaml` with correct filenames (case-sensitive)
- Perform full restart after adding assets (hot reload may not detect new files)
- Never commit API keys or secrets to version control
- Use environment variables or secure configuration files
- Provide example configuration files (e.g., `api_constants.example.dart`)
- Add sensitive files to `.gitignore`

---

## 🔌 API & ML Insights

### Key API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/auth/login` | User authentication |
| `POST` | `/api/auth/register` | User registration |
| `POST` | `/api/routines/generate` | Generate personalized routine |
| `GET` | `/api/routines/:userId` | Retrieve user routines |
| `PUT` | `/api/routines/feedback` | Provide ML feedback |

### Machine Learning Specifications

- **Model Type**: LSTM with Attention Mechanisms
- **Training Data**: 10k+ annotated routine samples
- **Accuracy**: 95% on validation set
- **Latency**: <200ms inference time
- **Deployment**: Google Cloud AI Platform
- **Retraining**: Weekly incremental learning from user feedback

### Example API Request
```bash
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
```

---

## 🎨 Visual Showcase

### Routine Dashboard
[View Dashboard on Notion](https://www.notion.so/IEEE-Competition-25842616b32780c8887bdf66c2312328)


### Design System
[Figma Design File](https://www.figma.com/design/kPoJr1Wk07ZCVCpYPbYFtn/NutriMind?node-id=0-1&p=f&t=KdJOqXrNztDiwGE9-0)

### Demo Video
[Watch Demo](https://drive.google.com/file/d/14Z2JcbXAJmLoI__lxf8WB0t54xOPCnId/view?usp=drive_link) 

---

## 🗺 Future Roadmap

### 2025 Q4
- [ ] Multilingual support (Arabic, Spanish, French)
- [ ] Wearable integration (Fitbit, Apple Health, Google Fit)
- [ ] Advanced sleep stage analysis

### Ongoing
- [ ] Community-driven features via in-app polls
- [ ] Enhanced model capabilities and accuracy

---

## 📄 License & Ethics

### License
MIT License - See LICENSE file for details

### Ethical Commitments
- **Transparent AI**: Open documentation of model capabilities and limitations
- **Bias Audits**: Regular testing for demographic and cultural biases
- **User Consent-First**: Explicit opt-in for data usage in model improvement
- **Privacy by Design**: End-to-end encryption for sensitive health data
- **Accessibility**: WCAG 2.1 compliance for users with disabilities

### Data Privacy
- User data never sold to third parties
- Anonymous aggregation for model improvement only with explicit consent
- Right to be forgotten with full data deletion capability

---

## 🤝 Contributing

We welcome contributions from the community! Please follow these steps to contribute:

### 1. Fork the Repository
Click the "Fork" button at the top right of the repository page to create your own copy.

### 2. Create a Feature Branch
```bash
git checkout -b feature/your-feature-name
```

### 3. Make Your Changes
Implement your feature or fix, following our coding standards and guidelines.

### 4. Commit and Push Your Changes
```bash
git add .
git commit -m "Add your descriptive commit message here"
git push origin feature/your-feature-name
```

### 5. Open a Pull Request
Navigate to the original repository and open a pull request, describing your changes in detail.

### Contribution Guidelines
- Follow the existing code style and architecture
- Write tests for new features
- Update documentation accordingly
- Ensure your code passes all existing tests
- Describe your changes clearly in the pull request

### Areas Where We Need Help
- UI/UX improvements
- Additional test coverage
- Documentation enhancements
- Performance optimizations
- Translation/localization

---

## 🙏 Acknowledgments

This journey has been more than just building a project—it has been a true test of our creativity, teamwork, and persistence. Our idea represents not only the solution we proposed, but also our ability to take a project from the ground up and bring it to life, from initial concept to hosting and running a full application.

We would like to express our deepest gratitude and appreciation to the **IEEE team** for organizing this remarkable competition. It has been an inspiring and unforgettable experience that allowed us to learn, grow, and collaborate while pushing the boundaries of what we can achieve together.

---

<div align="center">

**NutriMind AI** - Revolutionizing personal wellness through artificial intelligence


</div>
