# ATM Machine (Django)

A web-based ATM simulator built with Django. Users can sign up, log in and perform common ATM operations through a browser, with every action recorded in a transaction history.

## Features
- User sign up, login and logout
- Splash / welcome screen and dashboard
- Balance inquiry
- Deposit (add balance) and withdraw money
- Change password and password-reset pages
- Transaction history per user
- Ready for Heroku deployment (`Procfile`, `gunicorn`, `whitenoise`)

## Tech Stack
- Python, Django 3.1
- HTML / CSS templates
- SQLite (local) / PostgreSQL via `dj-database-url` (deployment)

## Project Structure
```
ATM-Machine-main/
├── atm/        # Django project settings, URLs, WSGI/ASGI
├── app/        # Core app: models, views, forms, URLs
├── atm_py/     # ATM UI app: templates (login, dashboard, balance...) and static CSS
├── Procfile    # Heroku process definition
└── requirements.txt
```

## Getting Started
```bash
cd ATM-Machine-main
python -m venv venv
venv\Scripts\activate          # Windows  (source venv/bin/activate on macOS/Linux)
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```
Open http://127.0.0.1:8000/ in your browser.

## Notes
This is a learning project; it is not a real banking system.