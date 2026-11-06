Hotel Reservation Prediction – MLOps

An end-to-end Machine Learning Operations (MLOps) project that predicts hotel reservation outcomes using machine learning.

Overview

This project uses a machine learning pipeline to process hotel reservation data, train a prediction model, and serve predictions through a Flask web application.

Tech Stack
Python
Pandas & NumPy
Scikit-learn
LightGBM
MLflow
Flask
Docker
Jenkins
Google Cloud Storage
Project Structure
text
├── artifacts/          # Model artifacts
├── config/             # Project configurations
├── custom_jenkins/     # Jenkins-related files
├── notebooks/          # Exploratory analysis
├── pipeline/           # ML training pipeline
├── src/                # Source code
├── static/             # Static web assets
├── templates/          # Flask HTML templates
├── utils/              # Utility functions
├── application.py      # Flask application
├── Dockerfile
├── Jenkinsfile
├── requirements.txt
└── setup.py

Installation & Usage
Clone the repository:
bash
git clone https://github.com/Shakestein/MLOPS-Hotel-Reservation.git
cd MLOPS-Hotel-Reservation

Create and activate a virtual environment:
bash
python -m venv venv
source venv/bin/activate

Install dependencies:
bash
pip install -r requirements.txt
pip install -e .

Run the application:
bash
python application.py

Open your browser and visit:
text
http://localhost:8080


Note: The application requires the trained model artifact at the configured model output path.

Docker

Build and run the Docker image:

bash
docker build -t hotel-reservation .
docker run -p 8080:5000 hotel-reservation

Author

Shakestein

GitHub Repository
