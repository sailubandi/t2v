# Talk2Invoice

## AI-Powered Voice Assistant for Food Ordering Using Whisper and DistilBERT

[![Python](https://img.shields.io/badge/Python-3.10+-blue)]()
[![AI Project](https://img.shields.io/badge/AI-Voice%20Ordering-success)]()
[![NLP](https://img.shields.io/badge/NLP-DistilBERT-orange)]()
[![Speech Recognition](https://img.shields.io/badge/STT-Faster%20Whisper-red)]()
[![Deployment](https://img.shields.io/badge/Deployment-HuggingFace-yellow)]()
[![License](https://img.shields.io/badge/License-Academic-lightgrey)]()

---

## Live Demo

### Hugging Face Deployment

[Try the Live Demo](https://huggingface.co/spaces/sailubandi/t2v)

### GitHub Repository

[View Source Code](https://github.com/sailubandi/t2v)

---

## Project Overview

Talk2Invoice is an AI-powered voice-based restaurant automation system designed to simplify food ordering, billing, inventory validation, and backend operations for fast-food restaurants, self-service kiosks, airports, metro stations, food courts, and other high-traffic service environments.

Instead of relying on manual counters or touchscreen systems, customers can place food orders using natural voice commands.

The system combines:

* OpenAI Whisper (Faster-Whisper) for multilingual Speech-to-Text conversion
* Fine-tuned DistilBERT for intent recognition and food item extraction
* Blockchain-based transaction logging for secure invoice generation
* Admin Dashboard for analytics, monitoring, and operational visibility

Once an order is captured, the system checks real-time inventory availability, validates kitchen workload, supports secure QR-based payment, and automatically generates digital invoices in PDF and HTML formats.

Talk2Invoice improves service speed, reduces human error, minimizes waiting time, and creates a seamless contactless ordering experience for modern restaurant environments.

---

## Abstract

Artificial Intelligence is transforming fast-food service environments by improving both customer experience and operational efficiency.

Traditional ordering systems often create problems such as:

* Long waiting queues
* Incorrect order placement
* Billing mistakes
* Delayed service during peak hours
* Heavy staff dependency
* Poor customer satisfaction

Talk2Invoice solves these challenges through an AI-powered voice assistant that enables contactless food ordering using natural speech.

Multilingual voice input is converted into text using Whisper, while customer intent and food item details are identified using a fine-tuned DistilBERT model.

QR code-based menu access simplifies ordering, while the backend system supports:

* Real-time inventory management
* Secure digital transactions
* Automated invoice generation
* Revenue reporting
* Business analytics

This creates a faster, smarter, and more reliable restaurant ordering system.

---

## Problem Statement

In restaurants, kiosks, airports, and food courts, customers often experience delays and confusion while placing orders using traditional systems.

### Existing Challenges

* Long waiting queues
* Incorrect order placement
* Slow service during rush hours
* Billing errors
* Limited multilingual support
* Poor voice recognition in noisy environments
* Lack of integration with inventory and billing systems

Most existing voice assistants fail because they cannot accurately understand natural speech in real-world restaurant environments and are not connected to backend systems like inventory validation and automated billing.

There is a strong need for an intelligent voice-based ordering platform that can:

* Understand customer intent
* Validate inventory in real time
* Reduce ordering errors
* Generate invoices automatically
* Improve service efficiency

Talk2Invoice is designed to solve this complete problem.

---

## Key Features

### Customer Features

* Voice-based food ordering
* Multilingual speech recognition
* Real-time Speech-to-Text conversion
* QR code-based menu access
* Natural language order placement
* Live order confirmation
* Cart review and modification
* Secure digital payment
* Automatic invoice generation
* PDF and HTML invoice download
* Contactless ordering experience

### Admin Features

* Real-time inventory management
* Kitchen workload balancing
* Daily sales monitoring
* Revenue analytics dashboard
* Top-selling item tracking
* Order validation monitoring
* Blockchain transaction visibility
* Stock update management
* Daily report generation

---

## Technology Stack

### Programming Language

* Python

### Machine Learning and AI

* OpenAI Whisper
* Faster-Whisper
* DistilBERT
* Hugging Face Transformers
* PyTorch
* Scikit-learn

### NLP and Speech Processing

* Speech-to-Text (STT)
* Text-to-Speech (gTTS)
* Google Gemini API
* Intent Recognition Pipeline

### Backend and Integration

* Gradio
* FastAPI
* Flask
* MongoDB
* JSON-based Persistent Storage

### Data Processing and Analytics

* Pandas
* NumPy
* Matplotlib
* Plotly
* ReportLab

### Security and Blockchain

* Blockchain Transaction Simulation
* Web3.py

### Deployment

* GitHub
* Hugging Face Spaces

---

## System Workflow

### Step 1: QR Code-Based Menu Access

Customer scans the QR code and opens the digital restaurant menu through the browser without needing mobile app installation.

### Step 2: Voice Input Collection

Customer places an order using natural speech.

Example:

"I want one pizza and two cold drinks"

### Step 3: Speech-to-Text Conversion

Faster-Whisper converts multilingual voice input into text accurately, even in noisy restaurant environments.

### Step 4: Intent Recognition

DistilBERT identifies:

* Food item names
* Quantity
* Modifiers
* Customer intent

Examples:

* Add order
* Remove item
* Modify order
* Finalize order

### Step 5: Inventory and Kitchen Load Validation

The system verifies:

* Item availability
* Stock levels
* Kitchen workload status

If unavailable, suitable alternatives are suggested.

### Step 6: Order Confirmation

The system confirms the detected order before final processing.

### Step 7: Secure Payment Processing

Customer completes QR-based secure digital payment.

### Step 8: Invoice Generation

The system automatically generates:

* PDF Invoice
* HTML Invoice

Invoice delivery methods:

* QR Code
* Email
* Download Option

### Step 9: Admin Monitoring and Analytics

Owner dashboard provides:

* Revenue reports
* Order tracking
* Stock monitoring
* Sales analytics
* Daily business insights
* Blockchain transaction records

---

## Installation Guide

### Step 1: Clone Repository

```bash
git clone https://github.com/sailubandi/t2v.git
cd t2v
```

### Step 2: Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate
```

For Windows:

```bash
venv\Scripts\activate
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Install FFmpeg

Required for Faster-Whisper audio processing.

Download from:

https://ffmpeg.org/download.html

### Step 5: Setup Environment Variables

Create a `.env` file

```env
GEMINI_API_KEY=your_api_key_here
```

### Step 6: Run Application

```bash
python app.py
```


## Sample Voice Commands

### Add Order

* Add one burger
* I want two pizzas
* Add three cold drinks

### Remove Order

* Remove one burger
* Cancel fries

### Finalize Order

* Finalize my order
* Confirm order

### Invoice Commands

* Generate invoice
* Show my bill

### General Queries

* What are today’s special items?
* Suggest available alternatives
* What is the price of pizza?

---

## Model Training and Evaluation

### DistilBERT Intent Recognition Model

The intent recognition system is built using a fine-tuned DistilBERT model trained on restaurant order datasets and customer conversational utterances.

### Training Configuration

* Batch Size: 32
* Optimizer: AdamW
* Learning Rate: 2e-5 to 5e-5
* Early Stopping: Enabled

### Evaluation Metrics

* Validation Accuracy
* Macro F1 Score

### Final Performance

**Validation Accuracy: 96.3%**

This ensures strong performance in:

* Noisy restaurant environments
* Multilingual conversations
* Natural food ordering requests
* Real-time customer interactions

---

## Testing Strategy

### Unit Testing

* Menu search validation
* Item mapping verification
* Invoice generation testing
* Order management validation

### Integration Testing

* Speech-to-Text testing
* Gemini command processing
* Text-to-Speech validation
* Language switching validation

### UI Flow Testing

* Customer login flow
* Order placement
* Payment completion
* Invoice download

### Scenario Testing

* Out-of-stock item handling
* Multilingual order placement
* Admin analytics verification
* Real-world restaurant order simulation

---

## Deployment

Talk2Invoice is deployed using Hugging Face Spaces.

### Advantages of Deployment

* Easy cloud hosting
* Automatic GitHub integration
* CPU and GPU runtime support
* Real-time model inference
* Simplified CI/CD workflow

### Continuous Integration and Deployment

Whenever code is pushed to GitHub:

* Automatic rebuild starts
* Latest version gets deployed
* No manual deployment required

This ensures a stable and production-ready deployment workflow.

---

## Future Scope

* Offline mode support
* Emotion detection from customer voice
* Swiggy integration
* Zomato integration
* AI-powered customer feedback analysis
* Voice-controlled kitchen monitoring
* Smart expiry-based food promotion
* Personalized recommendation engine
* Robotic food delivery integration

---

## Authors

### Project Lead

**Bandi Poorna Sri Sailaja**
B.Tech – Artificial Intelligence and Machine Learning
Sri Vasavi Engineering College



## Contact

### LinkedIn

https://linkedin.com/in/sailubandi

### GitHub

https://github.com/sailubandi

### Email

[sailubandi33@gmail.com](mailto:sailubandi33@gmail.com)

---

## Conclusion

Talk2Invoice is a complete AI-powered restaurant automation platform that combines:

* Voice Recognition
* Natural Language Processing
* Billing Automation
* Inventory Management
* Blockchain Security
* Admin Analytics

into one intelligent unified system.

It improves service speed, reduces manual errors, minimizes staff dependency, and delivers a seamless customer experience for modern restaurants and self-service environments.

This project demonstrates how Artificial Intelligence can transform traditional restaurant operations into scalable, smart, and future-ready digital food service systems.

---

## License

This project is developed for:

* Academic Purpose
* Research Purpose
* Learning Purpose
* Demonstration Purpose

---

