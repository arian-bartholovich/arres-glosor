# KFSCI23B Website

A full-stack community portal built for the **KFSCI23B Chemistry and Physics programme** at Europaskolan Strängnäs. The application brings class information, school news, fundraising links, and student interaction into one accessible web experience.

## Overview

This project demonstrates the ability to turn a real user community's needs into a structured web application. It combines a polished, content-driven front end with server-side routing, authentication, database persistence, and real-time communication.

## Features

- **Class and school hub** — presents programme information, school context, and class-focused content.
- **News experience** — provides dedicated pages for class events, including a futsal tournament, a Greece trip, and a sausage-eating competition.
- **User authentication** — supports registration, login, logout, session management, validation, and hashed passwords.
- **Real-time chat** — enables authenticated users to exchange messages through Socket.IO, with messages persisted in SQLite.
- **Protected content** — includes a controlled route for school documents.
- **Responsive visual interface** — uses reusable templates, static assets, Bootstrap components, and an image carousel to create an engaging user experience.
- **Fundraising integration** — links visitors to the class's NewBody fundraising campaign.

## Technical Highlights

| Area | Implementation |
| --- | --- |
| Backend | Python and Flask |
| Data | SQLite with CS50 SQL helpers |
| Authentication | Flask sessions and Werkzeug password hashing |
| Real-time communication | Flask-SocketIO |
| Front end | HTML, CSS, Jinja templates, Bootstrap |
| Application structure | Route-based Flask application with reusable layouts and static assets |

## What This Project Demonstrates

- Full-stack web development with Python and Flask
- Designing a usable product around a specific community
- Authentication and session-based access flows
- Relational data persistence and database queries
- Event-driven, real-time functionality with WebSockets
- Clear page architecture using reusable server-rendered templates
- Thoughtful visual presentation for a public-facing site

## Project Structure

```text
KFSCI23B-website/
├── app.py             # Flask routes, authentication, database, and Socket.IO events
├── functions.py       # Access-control decorators
├── information.db     # SQLite application data
├── static/            # Stylesheets, images, and client-side assets
└── templates/         # Reusable layouts and page templates
```

## Getting Started

1. Clone the repository.
2. Create and activate a Python virtual environment.
3. Install the project dependencies:

   ```bash
   pip install Flask Flask-Session Flask-SocketIO Flask-SQLAlchemy cs50
   ```

4. Set a `SECRET_KEY` environment variable for your local environment.
5. Start the application:

   ```bash
   python app.py
   ```

## Author

Developed by **Arian Bartholovich** as a practical full-stack web project for KFSCI23B at Europaskolan Strängnäs.
