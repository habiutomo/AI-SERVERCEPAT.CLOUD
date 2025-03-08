# AI SERVERCEPAT.CLOUD

![Python](https://img.shields.io/badge/python-3.11-blue.svg)
![Flask](https://img.shields.io/badge/flask-latest-green.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

![AI Chat Preview](ai.jpg)

Aplikasi chat berbasis web yang menggunakan Flask dan AIML API untuk membuat antarmuka chatbot yang mirip dengan GPT. Aplikasi ini menyediakan antarmuka yang user-friendly untuk berinteraksi dengan AI.

## Fitur

- 💬 Chat interface yang responsif dan modern
- 🌙 Dark mode theme yang nyaman di mata
- ⚡ Real-time chat dengan AI
- 🔄 Loading indicators untuk feedback visual
- 📱 Responsive design untuk desktop dan mobile
- 🔐 Sistem autentikasi pengguna

## Screenshot

<div align="center">
  <img src="https://raw.githubusercontent.com/servercepat/aichat/main/screenshots/login.svg" alt="Login Page" width="400"/>
  <img src="https://raw.githubusercontent.com/servercepat/aichat/main/screenshots/chat.svg" alt="Chat Interface" width="400"/>
</div>

## Teknologi yang Digunakan

- **Backend**: Python Flask
- **Frontend**: HTML, CSS, JavaScript
- **UI Framework**: Bootstrap
- **API**: AIML API untuk pemrosesan chat
- **Styling**: Custom CSS dengan Bootstrap dark theme
- **Database**: PostgreSQL

## Arsitektur Sistem

```mermaid
graph TD
    A[Client Browser] -->|HTTP/HTTPS| B[Flask Server]
    B -->|Authentication| C[PostgreSQL DB]
    B -->|API Requests| D[AIML API]
    D -->|AI Response| B
    B -->|Response| A
```

## Cara Menjalankan Aplikasi

1. Pastikan Python 3.11+ sudah terinstall
2. Install dependencies yang diperlukan:
   ```bash
   pip install flask requests python-dotenv gunicorn flask-login flask-sqlalchemy psycopg2-binary
   ```

3. Setup environment variables dalam file `.env`:
   ```
   AIML_API_KEY=your_api_key_here
   SESSION_SECRET=your_session_secret
   DATABASE_URL=your_database_url
   ```

4. Jalankan aplikasi:
   ```bash
   python main.py
   ```

5. Buka browser dan akses `http://localhost:5000`

## Environment Variables

- `AIML_API_KEY`: API key dari AIML API (Required)
- `SESSION_SECRET`: Secret key untuk Flask session (Required)
- `DATABASE_URL`: PostgreSQL database URL (Required)

## Struktur Proyek

```
.
├── models/
│   └── user.py
├── routes/
│   └── auth.py
├── static/
│   ├── css/
│   │   └── style.css
│   └── js/
│       └── chat.js
├── templates/
│   ├── auth/
│   │   ├── login.html
│   │   └── register.html
│   └── index.html
├── app.py
├── main.py
└── README.md
```

## Fitur yang Akan Datang

- [x] Sistem autentikasi pengguna
- [ ] Riwayat chat
- [ ] Penyimpanan percakapan
- [ ] Kustomisasi model AI

## Kontribusi

Silakan berkontribusi dengan membuat issue atau pull request jika ingin menambahkan fitur atau memperbaiki bug.

## Lisensi

MIT License habizinnia@gmail.com

## Author

[![AI SERVERCEPAT.CLOUD](https://img.shields.io/badge/AI-SERVERCEPAT.CLOUD-blue.svg)](https://servercepat.cloud)