# SKR Portfolio Chatbot — Backend

AI-powered portfolio chatbot for sangakarra.github.io/portfolio  
Built with Python, Flask, and Google Gemini API.

## Local Setup

1. Clone the repo
   git clone https://github.com/sangakarra/portfolio-chatbot.git
   cd portfolio-chatbot

2. Create virtual environment
   python3 -m venv venv
   source venv/bin/activate

3. Install dependencies
   pip install -r requirements.txt

4. Add your API key
   cp .env.example .env
   # Edit .env and add your Gemini API key

5. Run locally
   python app.py

   Server runs at http://localhost:5000

## API

POST /chat
Body: { "message": "Does he know Kafka?" }
Response: { "reply": "Yes, Sangarshan has hands-on experience with Apache Kafka..." }

## Deployment

Deployed on Render.com (free tier)
Set GEMINI_API_KEY as an environment variable in Render dashboard — never commit .env to GitHub.
