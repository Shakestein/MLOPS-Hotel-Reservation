Hotel Reservation Prediction – MLOps

An end-to-end MLOps project for predicting hotel reservation outcomes using machine learning.

Overview

This project demonstrates an end-to-end machine learning workflow, including data processing, model training, experiment tracking, and deployment through a Flask web application.

Tech Stack
Language: Python
Data Processing: Pandas, NumPy
Machine Learning: Scikit-learn, LightGBM
Experiment Tracking: MLflow
Backend: Flask
Containerization: Docker
CI/CD: Jenkins
Cloud Storage: Google Cloud Storage
Project Structure
text
MLOPS-Hotel-Reservation/
│
├── artifacts/          # Model artifacts
├── config/             # Configuration files
├── custom_jenkins/     # Jenkins-related files
├── notebooks/          # Jupyter notebooks
├── pipeline/           # ML pipelines
├── src/                # Source code
├── static/             # Static assets
├── templates/          # HTML templates
├── utils/              # Utility functions
│
├── application.py      # Flask application
├── Dockerfile          # Docker configuration
├── Jenkinsfile         # CI/CD pipeline
├── requirements.txt    # Dependencies
└── setup.py            # Package configuration

Installation

1. Clone the repository

bash
git clone https://github.com/Shakestein/MLOPS-Hotel-Reservation.git
cd MLOPS-Hotel-Reservation


2. Create a virtual environment

bash
python -m venv venv


3. Activate the environment

bash
# Windows
venv\Scripts\activate

# Linux / macOS
source venv/bin/activate


4. Install dependencies

bash
pip install -r requirements.txt
pip install -e .

▶️ Run the Application
bash
python application.py


Open your browser and visit:

text
http://localhost:8080


Ensure the required model artifacts and configuration are available before running the application.

Docker

Build the Docker image:

bash
docker build -t hotel-reservation .


Run the container (adjust the port mapping to match the port configured in the Dockerfile):

bash
docker run -p 8080:5000 hotel-reservation

Author

Shakestein

GitHub Repository

⭐ If you find this project useful, consider giving it a star!
