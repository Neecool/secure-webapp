# Secure Web Application (Flask)

A simple but secure web app demonstrating:

- User authentication (login/register)
- Password hashing with salt (Werkzeug)
- Role‑based authorization (user vs admin)
- SQL injection prevention (SQLAlchemy ORM)
- Session management (Flask-Login)

## Security features implemented (OWASP Top 10)

| OWASP Risk | Mitigation |
|------------|-------------|
| Broken Authentication | Strong password hashing, session mgmt |
| Sensitive Data Exposure | Passwords never stored in plain text |
| Injection | ORM prevents SQL injection |
| Broken Access Control | Role checks on admin routes |

## Setup

```bash
git clone https://github.com/Neecool/secure-webapp.git
cd secure-webapp
python -m venv venv
source venv/bin/activate   # or venv\Scripts\activate on Windows
pip install -r requirements.txt
python app.py
