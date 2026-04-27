```md id="m3z8rp"
# Talk2Invoice

## AI-Powered Voice Assistant for Food Ordering Using Whisper and DistilBERT

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue" />
  <img src="https://img.shields.io/badge/AI-Voice%20Ordering-success" />
  <img src="https://img.shields.io/badge/NLP-DistilBERT-orange" />
  <img src="https://img.shields.io/badge/STT-Faster%20Whisper-red" />
  <img src="https://img.shields.io/badge/Deployment-HuggingFace-yellow" />
  <img src="https://img.shields.io/badge/License-Academic-lightgrey" />
</p>

---

## Live Demo

### Hugging Face Deployment

🔗 [Try the Live Demo](https://huggingface.co/spaces/sailubandi/t2v)

### GitHub Repository

🔗 [View Source Code](https://github.com/sailubandi/t2v)

---

## Table of Contents

- [Project Overview](#project-overview)
- [Abstract](#abstract)
- [Problem Statement](#problem-statement)
- [Why This Project Matters](#why-this-project-matters)
- [Business Use Cases](#business-use-cases)
- [Key Features](#key-features)
- [Technology Stack](#technology-stack)
- [System Workflow](#system-workflow)
- [Installation Guide](#installation-guide)

---

## Project Overview

Talk2Invoice is an AI-powered voice-based restaurant automation system developed to simplify food ordering, billing, inventory validation, and backend operations for fast-food restaurants, self-service kiosks, airports, metro stations, food courts, and other high-traffic service environments.

Instead of relying on manual counters or touchscreen systems, customers can place food orders using natural voice commands.

The system combines:

- **OpenAI Whisper (Faster-Whisper)** for multilingual Speech-to-Text conversion
- **Fine-tuned DistilBERT** for intent recognition and food item extraction
- **Blockchain-based transaction logging** for secure invoice generation
- **Admin Dashboard** for analytics, monitoring, and operational visibility

Once an order is captured, the system checks real-time inventory availability, validates kitchen workload, supports secure QR-based payment, and automatically generates digital invoices in PDF and HTML formats.

Talk2Invoice improves service speed, reduces human error, minimizes waiting time, and creates a seamless contactless ordering experience for modern restaurant environments.

---

## Abstract

Artificial Intelligence is rapidly transforming fast-food service environments by improving customer experience and operational efficiency.

Traditional ordering systems often create problems such as:

- Long waiting queues
- Incorrect order placement
- Billing mistakes
- Delayed service during peak hours
- Heavy staff dependency
- Poor customer satisfaction

Talk2Invoice addresses these challenges through an AI-powered voice assistant that enables contactless food ordering using natural speech.

Multilingual voice input is converted into text using Whisper, while customer intent and food item details are identified using a fine-tuned DistilBERT model.

QR code-based menu access simplifies ordering, while the backend system supports:

- Real-time inventory management
- Secure digital transactions
- Automated invoice generation
- Revenue reporting
- Business analytics

This creates a faster, smarter, and more reliable restaurant ordering system.

---

## Problem Statement

In restaurants, kiosks, airports, and food courts, customers often experience delays and confusion while placing orders using traditional systems.

### Existing Challenges

- Long waiting queues
- Incorrect order placement
- Slow service during rush hours
- Billing errors
- Limited multilingual support
- Poor voice recognition in noisy environments
- Lack of integration with inventory and billing systems

Most existing voice assistants fail because they cannot accurately understand natural speech in real-world restaurant environments and are not connected to backend systems like inventory validation and automated billing.

There is a strong need for an intelligent voice-based ordering platform that can:

- Understand customer intent
- Validate inventory in real time
- Reduce ordering errors
- Generate invoices automatically
- Improve service efficiency

Talk2Invoice is designed to solve this complete problem.

---

## Why This Project Matters

The food service industry is rapidly moving toward:

- Contactless ordering
- Smart automation
- AI-powered customer service
- Faster operations
- Reduced manual dependency

Talk2Invoice helps restaurants modernize their operations while improving customer satisfaction and business profitability.

### Highly Relevant For

- Smart Restaurants
- Airport Food Counters
- Metro Station Food Kiosks
- Mall Food Courts
- Self-Service Restaurant Chains
- College Cafeterias

---

## Business Use Cases

### Fast Food Chains

Automated voice ordering reduces rush-hour delays and improves service speed.

### Airport Food Counters

Quick service for high-volume customer environments with minimal waiting time.

### Metro Station Kiosks

Low-latency ordering with minimal staff dependency.

### College Cafeterias

Self-service voice ordering with digital billing and faster queue handling.

### Cloud Kitchens

Automated order intake and smart invoice generation.

### Smart Restaurants

AI-powered operational analytics and customer service optimization.

---

## Key Features

### Customer Features

- Voice-based food ordering
- Multilingual speech recognition
- Real-time Speech-to-Text conversion
- QR code-based menu access
- Natural language order placement
- Live order confirmation
- Cart review and modification
- Secure digital payment
- Automatic invoice generation
- PDF and HTML invoice download
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

## Technology Stack

### Programming Language

- Python

### Machine Learning and AI

- OpenAI Whisper
- Faster-Whisper
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

### Deployment

- GitHub
- Hugging Face Spaces

---

## System Workflow

### Step 1: QR Code-Based Menu Access

Customer scans the QR code and opens the digital restaurant menu through the browser without needing mobile app installation.
```
