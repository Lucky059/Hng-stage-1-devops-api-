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


Endpoints:
GET /

json
{"message": "API is running"}
GET /health

json
{"message": "healthy"}
GET /me

json
{
  "name": "ukweku lucky",
  "email": "ukwekulucky@gmail.com",
  "github": "https://github.com/Lucky059"
}

☁️ Deployment Notes
Deploy on AWS EC2.

Use Nginx as a reverse proxy (port 80 → 8000).

Use systemd to keep the API alive after restarts.

✅ Testing
From any machine:

bash
curl http://your-ec2-public-ip/
curl http://your-ec2-public-ip/health
curl http://your-ec2-public-ip/me
