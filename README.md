````md
# Talk2Invoice: AI-Powered Voice Assistant for Food Ordering Using Whisper and DistilBERT

## Project Overview

Talk2Invoice is an AI-powered voice-based restaurant automation system developed to streamline food ordering, billing, and backend operations in fast-food restaurants, self-service kiosks, airports, metro stations, food courts, and high-traffic service environments.

The system enables customers to place food orders using natural voice commands instead of relying on manual counters or touchscreen systems. It uses OpenAI’s Whisper (Faster-Whisper) for multilingual Speech-to-Text conversion and a fine-tuned DistilBERT model for intent recognition and food entity extraction.

Once the order is captured, the system validates real-time inventory availability, checks kitchen workload, supports secure QR-based payment, and automatically generates digital invoices in PDF and HTML formats. A blockchain-enabled backend ensures transparent transaction logging and secure order records, while the admin dashboard provides business analytics, stock monitoring, and operational visibility.

Talk2Invoice improves service speed, reduces human error, minimizes waiting time, and creates a modern contactless food ordering experience suitable for real-world restaurant deployment.

---

## Live Deployment

### Hugging Face Space

https://huggingface.co/spaces/sailubandi/t2v

### GitHub Repository

https://github.com/sailubandi/t2v

---

## Abstract

Artificial Intelligence is increasingly being adopted in fast-food service environments to improve customer experience and operational efficiency. Traditional ordering systems often result in long queues, incorrect orders, billing errors, and reduced productivity during peak hours.

Talk2Invoice addresses these challenges through an AI-driven voice assistant that enables contactless food ordering using natural speech. Multilingual voice input is converted into text using Whisper, while customer intent and item details are identified using a fine-tuned DistilBERT model. QR code-based menu access simplifies interactions, and a blockchain-enabled backend supports real-time stock management, secure digital transactions, and automated invoice generation.

The system demonstrates improved order accuracy, reduced latency, and better transparency in restaurant operations by combining speech processing, NLP, backend automation, and secure transaction handling.

---

## Problem Statement

In fast-food places such as restaurants, kiosks, airports, and metro stations, customers frequently experience delays and confusion while placing orders using manual or touchscreen systems.

Existing systems suffer from:

- Long waiting queues
- Incorrect order placement
- Slow service during peak hours
- Billing mistakes
- Limited multilingual support
- Poor voice recognition in noisy environments
- Lack of backend integration with inventory and billing systems

Most existing voice assistants cannot accurately understand natural speech in real-world restaurant environments and are not connected to inventory validation or automated invoice generation.

To solve these issues, there is a need for an intelligent voice-based ordering system that can process natural speech, understand customer intent, validate orders in real time, and generate digital invoices automatically.

Talk2Invoice is developed to provide this complete AI-powered solution.

---

## Project Objectives

- Develop a voice-based food ordering assistant for restaurants
- Enable multilingual real-time Speech-to-Text conversion
- Improve order accuracy using Natural Language Processing
- Reduce customer waiting time and manual dependency
- Automate billing and invoice generation
- Improve inventory visibility and kitchen load management
- Provide business analytics through an admin dashboard
- Ensure secure and transparent transaction handling using blockchain simulation

---

## Key Features

## Customer Features

- Voice-based food ordering
- Multilingual speech recognition
- Real-time speech-to-text conversion
- QR code-based menu access
- Natural language order placement
- Live order confirmation
- Cart review and modification
- Secure digital payment support
- Automatic invoice generation
- PDF and HTML invoice download
- Contactless self-service ordering experience

---

## Admin Features

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

## Technology Stack

## Programming Language

- Python

---

## Machine Learning and Artificial Intelligence

- OpenAI Whisper
- Faster-Whisper
- DistilBERT
- Hugging Face Transformers
- PyTorch
- Scikit-learn

---

## Natural Language Processing and Speech Processing

- Speech-to-Text (STT)
- Text-to-Speech (gTTS)
- Google Gemini API
- Intent Recognition Pipeline

---

## Backend and System Integration

- Gradio
- FastAPI
- Flask
- MongoDB
- JSON-based Persistent Storage

---

## Data Processing and Analytics

- Pandas
- NumPy
- Matplotlib
- Plotly
- ReportLab

---

## Security and Blockchain

- Blockchain Transaction Simulation
- Web3.py

---

## Deployment and Version Control

- GitHub
- Hugging Face Spaces

---

## System Workflow

## Step 1: QR Code-Based Menu Access

The customer scans the restaurant QR code and opens the digital menu interface through the browser without requiring mobile app installation.

---

## Step 2: Voice Input Collection

The customer places an order using natural speech.

Example:

"I want one pizza and two cold drinks"

---

## Step 3: Speech-to-Text Conversion

The Faster-Whisper model converts multilingual voice input into text accurately, even in noisy restaurant environments.

---

## Step 4: Intent Recognition

The fine-tuned DistilBERT model identifies:

- Food item names
- Quantity
- Modifiers
- Customer intent

Examples:

- Add order
- Remove item
- Modify order
- Finalize order

---

## Step 5: Inventory and Kitchen Load Validation

The system verifies:

- Item availability
- Stock levels
- Kitchen workload status

If an item is unavailable, suitable alternatives are suggested.

---

## Step 6: Order Confirmation

The system confirms the detected order with the customer before final processing.

---

## Step 7: Secure Payment Processing

The customer completes QR-based secure digital payment.

---

## Step 8: Invoice Generation

The system automatically generates:

- PDF Invoice
- HTML Invoice

Invoice delivery methods:

- QR code
- Email
- Download option

---

## Step 9: Admin Monitoring and Analytics

The owner dashboard provides:

- Revenue reports
- Order tracking
- Stock monitoring
- Sales analytics
- Daily business insights
- Blockchain transaction records



## Installation Guide

## Step 1: Clone the Repository

```bash
git clone https://github.com/sailubandi/t2v.git
cd t2v
```

---

## Step 2: Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate
```

For Windows:

```bash
venv\Scripts\activate
```

---

## Step 3: Install Required Dependencies

```bash
pip install -r requirements.txt
```

---

## Step 4: Install FFmpeg

FFmpeg is required for Faster-Whisper audio processing.

Download:

https://ffmpeg.org/download.html

---

## Step 5: Configure Environment Variables

Create a `.env` file in the project root:

```env
GEMINI_API_KEY=your_api_key_here
```

---

## Step 6: Run the Application

```bash
python app.py
```

---

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

## DistilBERT Intent Recognition Model

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

Validation Accuracy: **96.3%**

This ensures strong performance in:

* Noisy restaurant environments
* Multilingual conversations
* Natural food ordering requests
* Real-time customer interactions

---

## Testing Strategy

The project includes:

## Unit Testing

* Menu search validation
* Item mapping verification
* Invoice generation testing
* Order management validation

---

## Integration Testing

* Speech-to-Text testing
* Gemini command processing
* Text-to-Speech validation
* Language switching validation

---

## UI Flow Testing

* Customer login flow
* Order placement
* Payment completion
* Invoice download

---

## Scenario Testing

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

## Project Lead

### Bandi Poorna Sri Sailaja

B.Tech – Artificial Intelligence and Machine Learning
Sri Vasavi Engineering College

---



---

## Conclusion

Talk2Invoice is a complete AI-powered restaurant automation system that combines:

* Voice Recognition
* Natural Language Processing
* Billing Automation
* Inventory Management
* Blockchain Security
* Admin Analytics

into one unified intelligent platform.

The system improves service speed, reduces manual errors, minimizes staff dependency, and delivers a seamless customer experience for modern restaurants and self-service environments.

It demonstrates how Artificial Intelligence can transform traditional restaurant operations into scalable, smart, and future-ready digital food service systems.

---

## License

This project is developed for:

* Academic Purpose
* Research Purpose
* Learning Purpose
* Demonstration Purpose

---

```
```
