# Smart Meeting Scheduler

A small FastAPI service and browser interface for finding shared free-time windows from participant busy slots.

## Features

- Accepts participant names and busy intervals for a selected date
- Intersects availability within a fixed 9:00 AM to 5:00 PM workday
- Filters windows by requested meeting duration
- Returns matching windows from `POST /api/schedule`

The app does not connect to calendar providers or book meetings; the page's booking button is a demonstration alert.

## Tech Stack

- **Backend:** Python, FastAPI, Pydantic
- **Frontend:** HTML, JavaScript, Tailwind CSS CDN

## Getting Started

Use Python 3.10 or later. From the repository root:

```bash
python -m venv .venv
```

Activate the environment, install the runtime packages, and start the API:

```bash
python -m pip install fastapi uvicorn
uvicorn main:app --reload
```

Open `index.html` in a browser while the API is running at `http://127.0.0.1:8000`.

## Author

Pasupuleti Neeraj

[GitHub](https://github.com/zero2006-lightnight) | [LinkedIn](https://www.linkedin.com/in/pasupuleti-neeraj-b0698a3a7)