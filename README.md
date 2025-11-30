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

**Notes**

- There is a database file `db.sqlite3` included for convenience (development only). Do not use this for production.
- I noticed a duplicate/typo file named `READEME.MD` in the same folder. If you want, I can remove or sync it with this `README.md`.

**Contributing**

If you want improvements or changes to the app, open an issue or submit a PR. For quick local changes, follow the Setup steps above.

**License**

This repository does not include a license file. If you want an open-source license added (MIT/Apache/etc.), tell me which one and I can add it.

---
If you'd like the README expanded (screenshots, deploy instructions, or CI setup), tell me what you'd like included.