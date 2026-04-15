# Hng-stage-1-devops-api-

## 📌 Overview
This is a simple FastAPI project built for the HNG DevOps Stage 1 task.  
It exposes three endpoints to demonstrate API deployment and cloud hosting.

## 🚀 How to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/Lucky059/Hng-stage-1-devops-api-.git
   cd Hng-stage-1-devops-api-
Create a virtual environment:

bash
python3 -m venv venv
source venv/bin/activate
Install dependencies:

bash
pip install fastapi uvicorn
Run the API:

bash
uvicorn main:app --reload --host 0.0.0.0 --port 8000
