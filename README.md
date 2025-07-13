# DynamicCV_Tool
Create a CV based on the Job Description to best allign with ATS


✨ AI-Powered Resume Tailoring Web App
This Flask web application allows users to upload their resume (.docx format) and tailor it for a specific job description using powerful AI models like OpenAI's GPT or DeepSeek. It generates an ATS-friendly, concise, and customized resume based on your input.

📂 Project Structure
cpp
Copy
Edit
├── app.py (Either OpenAI or DeepSeek version)
├── templates/
│   └── index.html
├── static/ (optional: CSS, JS)
├── requirements.txt
└── README.md
🚀 Features
Upload your resume (.docx) and paste a job description

Get a fully tailored, quantified, and ATS-optimized resume

Download output in .docx format

Choose between two backend models:

OpenAI GPT (Script 1)

DeepSeek LLM (Script 2)

🛠️ Requirements
Python 3.7+

pip install -r requirements.txt

txt
Copy
Edit
Flask
python-docx
openai          # For Script 1
requests        # For Script 2
💡 How It Works
Upload your existing resume in .docx format

Paste the job description

AI reads both and generates a tailored resume

You get a downloadable .docx version

🔐 Setup Instructions
⚙️ Script 1 — Using OpenAI GPT (gpt-3.5-turbo)
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
In app.py, replace the placeholder key:

python
Copy
Edit
openai.api_key = "***..."  # Replace with your OpenAI API key
Run the app:

bash
Copy
Edit
python app.py
⚠️ Avoid hardcoding API keys in production. Use environment variables instead.

⚙️ Script 2 — Using DeepSeek API
Set up your environment variable:

bash
Copy
Edit
export DEEPSEEK_API_KEY="your_api_key_here"
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the app:

bash
Copy
Edit
python app.py
✅ API key is safely read from os.environ.

🌐 Frontend
templates/index.html is a simple upload form with:

File input for .docx resume

Text area for job description

Submit button to trigger generation

🧠 Powered By
🧠 OpenAI ChatGPT (gpt-3.5-turbo)

🧠 DeepSeek LLM (deepseek-chat)

