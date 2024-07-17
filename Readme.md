# Flask User Authentication Application

This is a Flask application that allows users to sign up, sign in, and access a protected page. It includes user authentication, password validation, and navigation between pages.

## Features

- User Sign Up
- User Sign In
- Password Validation
  - Must contain at least one lowercase letter
  - Must contain at least one uppercase letter
  - Must end in a number
  - Must be at least 8 characters long
  - Can contain special characters
- Protected Page Access
- Flash Messages for User Feedback

## Requirements

- Python 3.6 or higher
- Flask
- Flask-SQLAlchemy
- Werkzeug

## Project Structure

```
Assignment07/
├── app.py
├── init_db.py
├── models.py
├── requirements.txt
├── templates/
│   ├── signup.html
│   ├── signin.html
│   ├── secretPage.html
│   ├── thankyou.html
└── static/
    └── styles.css
```

## Setup Instructions

### 1. Clone the repository

```bash
git clone <repository-url>
cd Assignment07
```

### 2. Create and activate a virtual environment

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Initialize the database

```bash
python init_db.py
```

### 5. Run the application

```bash
python app.py
```

### 6. Access the application

Open your web browser and navigate to `http://127.0.0.1:5000/`.

## File Descriptions

### `app.py`

This is the main application file that contains the route definitions and logic for user sign up, sign in, and protected page access.

### `models.py`

This file contains the SQLAlchemy model for the `User` table.

### `init_db.py`

This file initializes the database by creating the required tables.

### `requirements.txt`

This file lists the Python dependencies needed to run the application.

### `templates/signup.html`

This file contains the HTML template for the sign up page.

### `templates/signin.html`

This file contains the HTML template for the sign in page.

### `templates/secretPage.html`

This file contains the HTML template for the protected secret page.

### `templates/thankyou.html`

This file contains the HTML template for the thank you page after successful sign up.

### `static/styles.css`

This file contains the CSS styles for the HTML templates.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more information.
