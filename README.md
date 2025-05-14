# Fraud Detection System

An advanced real-time fraud detection system using machine learning and microservices architecture.

## Features
- Real-time transaction fraud detection
- Machine learning model with periodic retraining
- RESTful API interface
- PostgreSQL database for transaction storage
- Docker containerization
- Scalable architecture

## Setup
1. Clone the repository
2. Run `docker-compose up --build`
3. Access API at `http://localhost:8000`

## API Endpoints
- POST /transaction - Submit new transaction
- GET /statistics - Get fraud detection statistics
- POST /retrain - Trigger model retraining
