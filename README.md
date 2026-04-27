

```markdown
# Talk2Invoice
### AI-Powered Voice Assistant for Food Ordering Using Whisper and DistilBERT

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue" alt="Python">
  <img src="https://img.shields.io/badge/AI-Voice%20Ordering-success" alt="AI Project">
  <img src="https://img.shields.io/badge/NLP-DistilBERT-orange" alt="NLP">
  <img src="https://img.shields.io/badge/STT-Faster%20Whisper-red" alt="Speech Recognition">
  <img src="https://img.shields.io/badge/Deployment-HuggingFace-yellow" alt="Deployment">
  <img src="https://img.shields.io/badge/License-Academic-lightgrey" alt="License">
</p>

---

## 🚀 Live Demo

### Hugging Face Deployment
[Live Demo on Hugging Face](https://huggingface.co/spaces/sailubandi/t2v)

### GitHub Repository
[GitHub Repository](https://github.com/sailubandi/t2v)

---

## 📚 Table of Contents

- [Project Overview](#-project-overview)
- [Abstract](#-abstract)
- [Problem Statement](#-problem-statement)
- [Why This Project Matters](#-why-this-project-matters)
- [Business Use Cases](#-business-use-cases)
- [Key Features](#-key-features)
- [Technology Stack](#-technology-stack)
- [System Workflow](#-system-workflow)
- [Installation Guide](#-installation-guide)
- [Sample Voice Commands](#-sample-voice-commands)
- [Model Performance](#-model-performance)
- [Testing Strategy](#-testing-strategy)
- [Deployment](#-deployment)
- [Future Scope](#-future-scope)
- [Authors](#-authors)
- [Contact](#-contact)
- [Conclusion](#-conclusion)
- [License](#-license)

---

## 📌 Project Overview

Talk2Invoice is an AI-powered voice-based restaurant automation system developed to streamline food ordering, billing, inventory validation, and backend operations for fast-food restaurants, food courts, self-service kiosks, airports, metro stations, and high-traffic service environments.

The system enables customers to place food orders using natural voice commands instead of relying on manual counters or touchscreen systems.

### Core Technologies Used

- **OpenAI Whisper (Faster-Whisper)** for multilingual Speech-to-Text conversion
- **Fine-tuned DistilBERT** for intent recognition and food entity extraction
- **Blockchain-based transaction logging** for secure invoice generation
- **Admin Dashboard** for analytics, monitoring, and business visibility

Once the order is captured, the system validates real-time inventory availability, checks kitchen workload, processes secure QR-based payment, and automatically generates digital invoices in both PDF and HTML formats.

Talk2Invoice improves service speed, reduces human errors, minimizes waiting time, and creates a modern contactless food ordering experience suitable for real-world restaurant deployment.

---

## 🧠 Abstract

Artificial Intelligence is increasingly being adopted in fast-food service environments to improve customer experience and operational efficiency.

Traditional ordering systems often result in:
- Long queues
- Incorrect orders
- Billing errors
- Delayed service during peak hours
- Staff dependency
- Poor customer satisfaction

Talk2Invoice addresses these challenges using an AI-driven voice assistant that enables contactless food ordering through natural speech interaction.

Multilingual voice input is converted into text using Whisper, while customer intent and food item extraction are handled using a fine-tuned DistilBERT model.

QR code-based menu access simplifies ordering, while blockchain-enabled backend services support:
- Real-time stock management
- Secure digital transactions
- Automated invoice generation
- Revenue reporting
- Business analytics

This project demonstrates improved order accuracy, reduced latency, and better operational transparency by combining AI, NLP, speech processing, backend automation, and secure transaction handling.

---

## ❗ Problem Statement

In restaurants, food courts, airports, and kiosks, customers frequently face delays and confusion while placing food orders using traditional systems.

### Existing Problems
- Long waiting queues
- Incorrect order placement
- Slow service during rush hours
- Billing mistakes
- Limited multilingual support
- Poor voice recognition in noisy environments
- Lack of integration with inventory and billing systems

Most existing voice assistants fail because they cannot accurately understand natural speech in real-world restaurant environments and are not connected to backend operational systems.

There is a strong need for an intelligent voice-based ordering system that can:
- Understand customer intent
- Validate inventory in real time
- Reduce ordering errors
- Generate digital invoices automatically
- Improve service efficiency

Talk2Invoice is built to solve this complete problem.

---

## ⭐ Why This Project Matters

The food service industry is rapidly moving toward:
- Contactless ordering
- Smart automation
- AI-powered customer service
- Faster operations
- Reduced manual dependency

Talk2Invoice helps restaurants modernize operations while improving both customer satisfaction and business profitability.

### Highly Relevant For
- Smart Restaurants
- Airport Food Kiosks
- Metro Station Food Counters
- Mall Food Courts
- Self-Service Restaurant Chains
- Automated Cafeterias

---

## 🏢 Business Use Cases

- **Fast Food Chains:** Automated voice ordering reduces rush-hour delays.
- **Airport Food Counters:** Quick service for high-volume customer environments.
- **Metro Station Kiosks:** Low-latency ordering with minimal staff dependency.
- **College Cafeterias:** Self-service voice ordering with digital billing.
- **Cloud Kitchens:** Automated order intake and smart invoice generation.
- **Smart Restaurants:** AI-powered operational analytics and customer service.

---

## ✨ Key Features

### Customer Features
- Voice-based food ordering
- Multilingual speech recognition
- Real-time Speech-to-Text conversion
- QR code-based menu access
- Natural language order placement
- Live order confirmation
- Cart review and modification
- Secure digital payment
- Automatic invoice generation (PDF and HTML)
- Contactless ordering experience

### Admin Features
- Real-time inventory management
- Kitchen workload balancing
- Daily sales monitoring
- Revenue analytics dashboard
- Top-selling item tracking
- Order validation monitoring
- Blockchain transaction visibility
- Stock update management
- Daily report generation

---

## 🛠 Technology Stack

### Programming Language
- Python

### Machine Learning and AI
- OpenAI Whisper (Faster-Whisper)
- DistilBERT
- Hugging Face Transformers
- PyTorch
- Scikit-learn

### NLP and Speech Processing
- Speech-to-Text (STT)
- Text-to-Speech (gTTS)
- Google Gemini API
- Intent Recognition Pipeline

### Backend and Integration
- Gradio
- FastAPI
- Flask
- MongoDB
- JSON-based Persistent Storage

### Data Processing and Analytics
- Pandas
- NumPy
- Matplotlib
- Plotly
- ReportLab

### Security and Blockchain
- Blockchain Transaction Simulation
- Web3.py

---

## 🔄 System Workflow

1. **Step 1: QR Code Access** - Customer scans QR code for the digital menu.
2. **Step 2: Voice Input** - Customer speaks order (e.g., "I want one pizza").
3. **Step 3: Speech-to-Text** - Faster-Whisper converts audio to text.
4. **Step 4: Intent Recognition** - DistilBERT extracts items and quantities.
5. **Step 5: Validation** - System verifies stock and kitchen load.
6. **Step 6: Confirmation** - System confirms the order details.
7. **Step 7: Payment** - Secure QR-based digital payment.
8. **Step 8: Invoice Generation** - Automated PDF/HTML invoice delivery.
9. **Step 9: Admin Analytics** - Dashboard updates revenue and stock reports.

---

## ⚙ Installation Guide

### Step 1: Clone Repository
```bash
git clone [https://github.com/sailubandi/t2v.git](https://github.com/sailubandi/t2v.git)
cd t2v
```

### Step 2: Create Virtual Environment
```bash
python -m venv venv
# For Linux/macOS:
source venv/bin/activate
# For Windows:
venv\Scripts\activate
```

### Step 3: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 4: Install FFmpeg
Required for Faster-Whisper audio processing. Download from [FFmpeg.org](https://ffmpeg.org/download.html).

### Step 5: Setup Environment Variables
Create a `.env` file:
```env
GEMINI_API_KEY=your_api_key_here
```

### Step 6: Run Application
```bash
python app.py
```

---

## 🎤 Sample Voice Commands

- **Add Order:** "Add one burger", "I want two pizzas"
- **Remove Order:** "Remove one burger", "Cancel fries"
- **Finalize Order:** "Finalize my order", "Confirm order"
- **Queries:** "What are today’s special items?", "What is the price of pizza?"

---

## 📈 Model Performance

### DistilBERT Intent Recognition Model
- **Training Configuration:** Batch Size 32, AdamW Optimizer, LR 2e-5.
- **Validation Accuracy:** **96.3%**
- **Capabilities:** Reliable in noisy environments and multilingual contexts.

---

## 🧪 Testing Strategy

- **Unit Testing:** Menu search, item mapping, and invoice generation.
- **Integration Testing:** STT to Gemini command processing flow.
- **UI Flow Testing:** Login, order placement, and payment completion.
- **Scenario Testing:** Out-of-stock handling and multilingual simulation.

---

## ☁ Deployment

Talk2Invoice is deployed using **Hugging Face Spaces**.
- **Benefits:** Automatic CI/CD, GitHub integration, and real-time model inference.

---

## 🔮 Future Scope

- Offline mode support
- Emotion detection from customer voice
- Swiggy and Zomato integration
- AI-powered customer feedback analysis
- Voice-controlled kitchen monitoring
- Personalized recommendation engine
- Robotic food delivery integration

---

## 👩‍💻 Authors

**Project Lead**
**Bandi Poorna Sri Sailaja**
B.Tech – Artificial Intelligence and Machine Learning
Sri Vasavi Engineering College

---

## 📬 Contact

- **LinkedIn:** [linkedin.com/in/sailubandi](https://linkedin.com/in/sailubandi)
- **GitHub:** [github.com/sailubandi](https://github.com/sailubandi)
- **Email:** sailubandi33@gmail.com

---

## 🏁 Conclusion

Talk2Invoice is a complete AI-powered restaurant automation platform that combines Voice Recognition, NLP, Billing Automation, Inventory Management, Blockchain Security, and Admin Analytics into one intelligent unified system. It improves service speed, reduces manual errors, and delivers a seamless customer experience for modern food service environments.

---

## 📄 License

This project is developed for Academic, Research, Learning, and Demonstration Purposes.
```
