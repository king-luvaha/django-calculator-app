# Django Calculator App

A simple calculator web application built with Django. This project demonstrates Django’s project structure, web form handling, and arithmetic operations in a web environment.

---

## Preview

![PREVIEW](dca.gif)

---
## Folder Structure

```
django-calculator-app/
├── djangoprojects/            # Calculator logic (views, URLs)
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
│   ├── rootapp/               # Home and base routing
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
│   ├── templates/             # HTML templates
│   │   └── calculatorapp/
│   ├── db.sqlite3             # SQLite database
│   └── manage.py              # Django management script
├── venv/                      # Python virtual environment
├── .gitignore
└── requirements.txt           # Project dependencies
```

---

## 🚀 Features

- Evaluate arithmetic expressions securely.
- Handles parentheses, operator precedence, and invalid inputs.
- Clean and responsive frontend using Bootstrap.
- Organized with reusable Django apps.

---

## Getting Started

### Installation

1. **Clone this repository:**
   ```bash
   git clone https://github.com/king-luvaha/django-calculator-app.git
   cd django-calculator-app/djangoprojects
   ```

2. **Create and activate a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**

   ```bash
   pip install -r ../requirements.txt
   ```

   If you don’t have a `requirements.txt` file, you can generate one:

   ```bash
   pip freeze > ../requirements.txt
   ```


4. **Run Database Migrations:**
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

## 🌐 View the Calculator

Once the server is running, **go to your browser** and open:

```
http://localhost:8000/calculatorapp
```

This will take you directly to the calculator interface.

If you're unsure, check the terminal output for:

```
Starting development server at http://127.0.0.1:8000/
```

Then manually navigate to `/calculatorapp`.

---

## 📦 Expression Logic

The calculator uses Python’s `ast` module to safely parse and evaluate expressions without the security risks of `eval()`. It only supports:

- Addition `+`
- Subtraction `-`
- Multiplication `*`
- Division `/`
- Parentheses `( )`

---

## 🧪 Example Usage

**Input:**

```
(2 + 3) * 4 - 7 / (1 + 1)
```

**Output:**

```
18.5
```

Invalid expressions like `2 +` or `5 / 0` are handled with user-friendly error messages.

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

