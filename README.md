# Insurance-Prediction-API-FastAPI-

# 📌 Overview

The Insurance Premium Prediction API is a machine learning–powered backend service that predicts the insurance premium category of a user based on demographic, lifestyle, and financial attributes.

The system uses a Random Forest Classifier (scikit-learn) trained on structured data and exposes real-time predictions through a FastAPI-based REST API. The application is fully containerized using Docker for reproducible and consistent deployments.

# 🚀 Features

✅ Random Forest model for classification

✅ Real-time prediction via FastAPI

✅ Input validation using Pydantic

✅ Automatic BMI, age group, and lifestyle risk computation

✅ Probability distribution for all premium categories

✅ Dockerized for seamless deployment

# 🧠 Model Details

Algorithm: Random Forest Classifier

Library: scikit-learn

Serialization: Pickle

Output:

Predicted premium category

Confidence score

Probability distribution across all classes

The model processes engineered features such as:

BMI (computed from height & weight)

Age group classification

Lifestyle risk assessment

City tier categorization

Income level

Occupation type

# 🛠 Tech Stack

Backend: FastAPI

Validation: Pydantic

ML: scikit-learn, pandas, NumPy

Containerization: Docker

Language: Python

# 📡 API Endpoints
🔹 GET /

Returns basic API information.

🔹 GET /health

Health check endpoint returning:

# API status

Model version

Model load status

# 🔹 POST /predict

Accepts user data and returns:

Predicted insurance category

Confidence score

Class probability distribution

# 🐳 Docker Support

The application is containerized using Docker to ensure:

Environment consistency

Dependency isolation

Easy deployment across systems

# 🚀 How to Run the Project

1️⃣ Pull from Docker Hub
docker pull rosypaul/insurance-premium-api
2️⃣ Run the Container
docker run -p 8000:8000 rosypaul/insurance-premium-api

The API will now be available at:

http://localhost:8000

# 📡 API Documentation

Once the server is running, visit:

http://localhost:8000/docs

This opens the interactive Swagger UI, where you can:

Test the /predict endpoint

Provide sample input

View real-time model responses
