<p align="center">
  <img src="assets/logo.png"/>
  <h1 align="center">Fundusnap</h1>
</p>

Fundusnap is a comprehensive medical imaging solution designed to help healthcare professionals detect and analyze diabetic retinopathy through fundus images. The project consists of three main components: a mobile application, a backend API service, and an AI model for offline image classification.

## 🏥 Project Components

### 1. Fundusnap Mobile App ([fundusnap-app](https://github.com/digination-alfamale-itb/fundusnap-app))
A modern cross-platform mobile application built with Flutter that provides:
- High-quality fundus image capture
- Video recording capabilities
- Secure storage of medical images
- AI-powered analysis of diabetic retinopathy
- Intelligent chatbot assistant for medical insights

**Tech Stack:**
- Framework: Flutter (SDK ^3.8.0)
- Language: Dart
- State Management: Flutter Bloc
- Navigation: Go Router
- Key Dependencies:
  - Camera: `camera: ^0.11.1`
  - Video Player: `video_player: ^2.9.5`
  - Secure Storage: `flutter_secure_storage: ^9.2.4`
  - Image Picker: `image_picker: ^1.1.2`
  - HTTP Client: `dio: ^5.8.0+1`

### 2. Fundusnap API ([fundusnap-api](https://github.com/digination-alfamale-itb/fundusnap-api))
A robust backend service that handles:
- User authentication and management
- Image analysis and processing
- AI-powered chat interactions
- Secure storage of medical data
- HIPAA-compliant data handling

**Tech Stack:**
- Runtime: Node.js
- Framework: Express.js
- Database: MongoDB with Mongoose
- Authentication: JWT
- Storage: Azure Blob Storage
- AI Services:
  - Microsoft Azure Custom Vision API
  - OpenRouter API with Microsoft MAI-DS-R1 model
- Email Service: Nodemailer

### 3. Fundusnap AI ([fundusnap-ai](https://github.com/digination-alfamale-itb/fundusnap-ai))
An offline-capable image classification system that serves as a fallback solution for:
- Offline image analysis
- Poor network connectivity scenarios
- Primary API unavailability

**Tech Stack:**
- Deep Learning Framework: FastAI
- Base Model: ResNet34 (pretrained)
- Data Augmentation: Albumentations
- Loss Function: Focal Loss
- Performance Metrics:
  - Overall Accuracy: 81%
  - Macro Average F1-Score: 0.81
  - Weighted Average F1-Score: 0.81

## 🔒 Security & Compliance

The entire system is designed with security and compliance in mind:
- HIPAA-compliant data storage and handling
- Secure authentication using JWT
- Encrypted data transmission
- Secure storage of medical images
- Regular security updates and patches

## 🚀 Getting Started

Each component has its own repository with detailed setup instructions. Please refer to the individual README files in each repository for specific setup and installation steps.

## 📝 License

This project is licensed under the MIT License.

## 👥 Authors

Fundusnap Developers <dev@fundusnap.com>
