# Arres Glosor

**Arres Glosor** is a full-stack vocabulary-learning platform that lets users create, organize, and practise their own language exercises. Built with Django, it combines an intuitive study workflow with account-based ownership, persistent data, and dynamic JSON-powered updates.

## Overview

The project was designed around a clear learner need: make vocabulary practice more flexible than a fixed word list. Users can build exercises for any two languages, manage translations, review a complete exercise, and switch the study direction as they practise.

## Features

- **Custom vocabulary exercises** — create named exercises for any language pair.
- **Translation management** — add and remove vocabulary pairs within an exercise.
- **Bidirectional practice** — switch the active language direction while studying.
- **Personal learning library** — browse exercises ordered by latest update and view creator profiles.
- **User authentication** — register, log in, and log out using Django’s authentication framework.
- **Ownership controls** — exercise editing is limited to the user who created it.
- **Persistent data model** — stores exercise details, timestamps, creators, and translation pairs in SQLite.
- **Dynamic interface** — uses JSON requests and responses for responsive create, save, and delete actions.

## Technical Highlights

| Area | Implementation |
| --- | --- |
| Framework | Django 5 |
| Language | Python |
| Database | SQLite with Django ORM |
| Authentication | Custom Django user model and built-in authentication tools |
| Data design | Relational `Exercise` model with JSON-based translation storage |
| Front end | Django templates, HTML, CSS, and JavaScript |
| Deployment support | Gunicorn, WhiteNoise, and Vercel configuration |

## What This Project Demonstrates

- Building a user-centered learning product from concept to implementation
- Designing server-side routes and reusable Django templates
- Implementing registration, login, logout, and access-aware editing flows
- Modeling relational data with Django ORM and foreign-key ownership
- Building JSON endpoints to support responsive client-side interactions
- Handling validation, error states, and missing resources
- Designing a flexible data model that supports many language combinations

## Project Structure

```text
arres-glosor/
├── arres_glosor/       # Django app: models, routes, views, templates, and static assets
├── final_project/      # Django project settings and deployment entry points
├── db.sqlite3          # Local SQLite database
├── manage.py           # Django command-line entry point
├── requirements.txt    # Python dependencies
└── vercel.json         # Deployment configuration
```

## Getting Started

1. Clone the repository and enter the project folder.
2. Create and activate a virtual environment.
3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Apply database migrations:

   ```bash
   python manage.py migrate
   ```

5. Start the development server:

   ```bash
   python manage.py runserver
   ```

6. Open `http://127.0.0.1:8000` in your browser.

## Author

Developed by **Arian Bartholovich** as a full-stack Django application that pairs thoughtful learning design with robust web development fundamentals.
