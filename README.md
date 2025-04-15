# ✈️ FormPilot

**FormPilot** is a lightweight, self-hosted form builder that lets users create embeddable forms and receive submissions via their own SMTP email setup. No external email API required.

## 🚀 Features

- 🔐 User authentication (Flask + React)
- 📝 Create and manage custom forms
- 📩 Send form submissions to your email via your SMTP settings
- 🌐 Shareable public form URLs
- 📊 Submission logs (coming soon)
- 🎨 (Planned) Embeddable form widgets and custom branding

---

## 🧱 Stack

- **Frontend:** React + Tailwind CSS
- **Backend:** Python Flask (REST API)
- **Database:** MySQL
- **Email:** SMTP via user-provided credentials (e.g., Gmail App Password)

---

## 🛠️ Local Development

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/formpilot.git
cd formpilot
```

### 2. Set up the backend

```bash
cd backend
python -m venv venv
source venv/bin/activate  # or .\venv\Scripts\activate on Windows
pip install -r requirements.txt

# Add your .env config
cp .env.example .env

# Run the Flask API
flask run
```

### 3. Set up the frontend

```bash
cd frontend
npm install
npm run dev
```

### .env Configuration

```env
SECRET_KEY=your_secret_key
MYSQL_USER=root
MYSQL_PASSWORD=your_password
MYSQL_HOST=localhost
MYSQL_DB=formpilot

# Optional default SMTP fallback (for testing)
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
```

## 🧪 Coming Soon

- Form analytics dashboard
- Submission storage and export
- File uploads
- Embeddable script snippet
- Optional email fallback via Resend/Postmark

## 💡 Inspiration

Built to solve the problem of receiving form submissions without relying on external services like Formspree, Typeform, or email APIs. Perfect for freelancers, creators, or developers looking for a quick solution that they control.

## 🛫 Ready to fly?

Start building forms, drop them anywhere, and let FormPilot handle the delivery. ✉️

MIT License
