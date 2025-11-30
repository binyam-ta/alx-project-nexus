# alx-project-nexus

A small Django "Polls" application used for learning and demonstration purposes.

**Quick summary**

- **What:** A simple Django project that implements a polling app (list polls, vote, view results).
- **Stack:** Python, Django, SQLite (default development DB).

**Features**

- View available polls on the index page.
- Vote on a poll and see live results.
- Admin interface for creating polls and choices.

**Prerequisites**

- Python 3.8 or newer
- pip
- (optional) virtualenv or venv

**Setup (local development)**

1. Create and activate a virtual environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

2. Install dependencies

If the project has a `requirements.txt` file use:

```bash
pip install -r requirements.txt
```

If there is no `requirements.txt`, install Django directly:

```bash
pip install django
```

3. Run migrations and start the dev server

```bash
python manage.py migrate
python manage.py createsuperuser   # optional, to use the admin
python manage.py runserver
```

Open http://127.0.0.1:8000/ in your browser to see the app.

**Running tests**

```bash
python manage.py test
```

**Project layout (important files)**

- `manage.py` - Django CLI entrypoint
- `db.sqlite3` - SQLite database (development)
- `polls/` - Django project settings and configuration
- `pollsapp/` - The polls application (models, views, templates, static files)
	- `pollsapp/templates/` - HTML templates: `index.html`, `vote.html`, `result.html`
	- `pollsapp/static/` - Static assets (CSS)






---
