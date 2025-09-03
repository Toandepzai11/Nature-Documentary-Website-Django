# Django Project: Trinh Huu Phuc Toan's Website

## Overview
This project is built with Django and contains two main applications:

- **app**: Core website with homepage and extended pages featuring a dynamic navigation bar.
- **accounts**: Manages user authentication (signup and login) with user data stored in a Supabase database.

## Project Structure
- **app**: Contains the main template (`base.html`) with a dynamic navbar that updates based on user login status.
- **accounts**: Handles user registration and login.

## Setup

### Prerequisites
Install Django:
```bash
pip install django
```
### Database Configuration
This project uses Supabase (PostgreSQL). Extract the following from your Supabase connection string and add them to `settings.py` under `DATABASES`:

- `DATABASE_NAME`: Last part of the connection string
- `USER`: Before the first `:`
- `PASSWORD`: Between the first `:` and `@`
- `HOST`: Between `@` and the next `:`
- `PORT`: Usually `5432`

### Installed Apps
Add `app` and `accounts` to `INSTALLED_APPS` in `settings.py`.

### URL Configuration
Include the `accounts` app URLs in the main `urls.py`.

### Templates
The `base.html` template in the `app` directory contains the site layout and dynamic navbar.

### Running the Project

Apply migrations:
```bash
python manage.py migrate
```
Create superuser:
```bash
python manage.py createsuperuser
```
Run the development server:
```bash
python manage.py runserver
```
Access the website at: http://127.0.0.1:8000/
### Notes
- Uses Django's built-in authentication system.
- Ensure templates and static files are configured properly.
