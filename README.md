
# Wiki — CS50W Project 0

A Wikipedia-like encyclopedia built with Django, where users can create, edit, and search for encyclopedia entries written in Markdown.

## Demo

[![Watch the demo](https://img.shields.io/badge/YouTube-Watch%20Demo-red?logo=youtube)](https://youtu.be/Z3Q2EeGHUD0?si=l6-hADsEvaBzCRjQ)

## Features

- **Entry pages** — each encyclopedia entry is rendered from a Markdown file into HTML
- **Index page** — lists all available entries with links to each
- **Search** — substring search that shows matching entries or redirects directly if exact match found
- **New entry** — create entries using a Markdown editor with duplicate detection
- **Edit entry** — pre-populated form to edit any existing entry's Markdown content
- **Random page** — navigate to a randomly selected encyclopedia entry

## Tech Stack

- **Backend** — Python, Django
- **Templating** — Django Templates
- **Content format** — Markdown (converted to HTML via `python-markdown2`)
- **Styling** — CSS, Bootstrap

## Project Structure

```
wiki/
├── encyclopedia/
│   ├── templates/encyclopedia/   # HTML templates
│   ├── static/encyclopedia/      # CSS and static assets
│   ├── entries/                  # Markdown files for each entry
│   ├── urls.py
│   ├── views.py
│   └── util.py                   # Helper functions (get/save/list entries)
├── wiki/
│   ├── settings.py
│   └── urls.py
│ ── db.sqlite3
└── manage.py
```

## Setup

```bash
git clone https://github.com/YOUR_USERNAME/wiki.git
cd wiki
pip install -r requirements.txt
python manage.py runserver
```

Then visit `http://127.0.0.1:8000`.

## Course

[CS50's Web Programming with Python and JavaScript](https://cs50.harvard.edu/web/) — Project 0

.
