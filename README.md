# Event Resource Allocation

Event Resource Allocation is a small Flask app for event scheduling and resource allocation. It provides a simple UI to create events, register resources, allocate resources to events, and generate utilization reports.

## Features
- User registration and login
- Create and list events with start/end times and descriptions
- Add and list resources (e.g. rooms, equipment)
- Allocate resources to events with conflict detection
- Generate a resource utilization report
- Responsive, purple-themed UI with a landing hero page

## Tech Stack
- Python 3.10+
- Flask
- PyMongo (MongoDB)
- Jinja2 templates
- Static CSS in `static/css/style.css`

## Project Structure
```
EventResourceAllocation/
├─ app.py
├─ templates/
│  ├─ base.html
│  ├─ index.html
│  ├─ login.html
│  └─ ...
├─ static/
│  └─ css/style.css
└─ README.md
```

## Quickstart (Windows)
1. Create a venv and activate it:

```cmd
python -m venv venv
venv\Scripts\activate
```

2. Install dependencies (create `requirements.txt` or install directly):

```cmd
pip install flask pymongo werkzeug
```

3. Create a `.env` file in the project root (or set environment variables):

```
FLASK_SECRET_KEY=your-secret-key
MONGODB_URI=mongodb://localhost:27017
```

4. Run the app:

```cmd
python app.py
```

5. Open `http://127.0.0.1:5000/` in your browser.

## Environment variables
- `FLASK_SECRET_KEY` — session secret key
- `MONGODB_URI` — MongoDB connection string

## UI / Styling Notes
- Primary color: **purple** (variables in `static/css/style.css`)
- Landing hero page at `/` (`templates/index.html`)
- Forms and tables are styled consistently via the stylesheet

## Endpoints
- `/` — Landing hero page (redirects signed-in users to `/events`)
- `/register` — Create a new user
- `/login` — Login
- `/events` — Create and list events
- `/resources` — Add and list resources
- `/allocate` — Allocate resource to an event
- `/report` — Generate utilization report

## Contributing
Contributions welcome — create an issue or a PR with fixes or improvements.

## License
MIT License


Snippets

<img width="1920" height="1200" alt="Screenshot (543)" src="https://github.com/user-attachments/assets/1694b497-6188-464f-91ed-596913669568" />

<img width="1920" height="1200" alt="Screenshot (544)" src="https://github.com/user-attachments/assets/05f6e8c8-9a87-459e-beda-f53966bc3625" />

<img width="1920" height="1200" alt="Screenshot (545)" src="https://github.com/user-attachments/assets/e6c0f705-10b1-49aa-8e89-a397a97962e6" />

<img width="1920" height="1200" alt="Screenshot (546)" src="https://github.com/user-attachments/assets/ce504c40-21c6-4770-9803-9c9844d42d14" />

<img width="1920" height="1200" alt="Screenshot (547)" src="https://github.com/user-attachments/assets/d1f62044-e34d-438c-b1c6-480713152b4c" />

<img width="1920" height="1200" alt="Screenshot (548)" src="https://github.com/user-attachments/assets/a1484207-b67f-4ec5-ab9d-b1dc951f753c" />

<img width="1920" height="1200" alt="Screenshot (549)" src="https://github.com/user-attachments/assets/7beb00be-f946-4139-b2b9-024daf814689" />



Recorded video -(https://drive.google.com/file/d/112ph9KB9gaXQZQ8k21ciRa8gI0pYb5WQ/view?usp=sharing)

