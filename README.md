# Django Calculator App

A simple calculator web application built with Django. This project demonstrates Django’s project structure, web form handling, and arithmetic operations in a web environment.

---

## Folder Structure

```
django-calculator-app/
├── djangoprojects/
│   ├── calculatorapp/
│   │   ├── migrations/
│   │   ├── __init__.py
│   │   ├── admin.py
│   │   ├── apps.py
│   │   ├── models.py
│   │   ├── tests.py
│   │   ├── urls.py
│   │   └── views.py
│   ├── djangoprojects/
│   │   ├── __init__.py
│   │   ├── asgi.py
│   │   ├── settings.py
│   │   ├── urls.py
│   │   └── wsgi.py
│   ├── rootapp/
│   │   ├── migrations/
│   │   ├── __init__.py
│   │   ├── admin.py
│   │   ├── apps.py
│   │   ├── models.py
│   │   ├── tests.py
│   │   ├── urls.py
│   │   └── views.py
│   ├── static/
│   │   └── main.jpg
│   ├── templates/
│   │   └── calculatorapp/
│   ├── db.sqlite3
│   └── manage.py
├── venv/
├── .gitignore
└── requirements.txt
```

---

## Features

- Perform basic arithmetic operations: addition, subtraction, multiplication, division
- Clean, user-friendly web interface
- Follows Django best practices with reusable apps

---

## Getting Started

### Prerequisites

- Python 3.8+
- pip (Python package manager)
- (Recommended) virtualenv

### Installation

1. **Clone this repository:**
   ```bash
   git clone https://github.com/king-luvaha/django-calculator-app.git
   cd django-calculator-app/djangoprojects
   ```

2. **(Optional) Create and activate a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r ../requirements.txt
   ```

4. **Run migrations:**
   ```bash
   python manage.py migrate
   ```

5. **Run the development server:**
   ```bash
   python manage.py runserver
   ```

6. **Access the app:**
   - Open your browser at [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

---

## Usage

- Enter numbers and select an arithmetic operation on the web interface.
- View the result displayed instantly.

---

## Project Structure Explained

- `calculatorapp/`: Main app for calculator logic and views.
- `rootapp/`: Additional Django app (purpose may vary; extend as needed).
- `djangoprojects/djangoprojects/`: Django project settings and configuration.
- `static/`: Static files (e.g., images).
- `templates/`: HTML templates for the calculator app.
- `db.sqlite3`: Default SQLite database (auto-generated).
- `requirements.txt`: Python dependencies.
- `manage.py`: Django’s CLI utility.

---

## Contributing

Contributions are welcome! Please open an issue or pull request.

1. Fork the repository
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -am 'Add feature'`)
4. Push to your branch (`git push origin feature/YourFeature`)
5. Open a pull request

---

## License

This project is open source. See the [LICENSE](LICENSE) file for details.

---

