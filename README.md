# ⏳ Deadline Tracker

An AI-powered web application built with Streamlit and Gemini Vision that automatically extracts dates, events, and deadlines from uploaded documents, timetables, or photos, and sends structured summaries directly to WhatsApp via Twilio.

---

## 🚀 Features

- 📄 **Multimodal Extraction:** Accepts images (JPG, JPEG, PNG) and PDFs (syllabi, timetables, assignment sheets).
- 🧠 **Gemini Vision Processing:** Automatically parses and extracts key dates and deadlines.
- 💬 **Interactive Chat Interface:** Query your deadlines and ask follow-up questions.
- 📱 **WhatsApp Integration:** Send deadline summaries straight to your WhatsApp account via Twilio API.

---

## 📂 Project Structure
  text
deadline-tracker/
├── app.py                  # Main Streamlit application
├── requirements.txt        # Python dependencies
├── .gitignore              # Ignored files (secrets, venv)
└── .streamlit/
    └── secrets.toml        # API Keys & Credentials (Local only)

 
 
🛠️ Local Setup & Installation
1. Clone the Repository
git clone [https://github.com/your-username/deadline-tracker.git](https://github.com/your-username/deadline-tracker.git)
cd deadline-tracker

2. Create & Activate Virtual Environment
python -m venv venv

3. Install Dependencies
pip install -r requirements.txt

4. Set Up API Credentials
Create a file named secrets.toml inside the .streamlit/ folder and add your credentials:

Ini, TOML
GEMINI_API_KEY = "your_actual_gemini_api_key"
TWILIO_ACCOUNT_SID = "your_actual_twilio_account_sid"
TWILIO_AUTH_TOKEN = "your_actual_twilio_auth_token"
TWILIO_WHATSAPP_FROM = "whatsapp:+14155238886"
TWILIO_CONTENT_SID = "your_actual_twilio_content_sid"

⚠️ Security Note: Never commit your .streamlit/secrets.toml to GitHub. Ensure it is included in your .gitignore.

🏃 Run the Application
streamlit run app.py
