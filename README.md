# Commerce — CS50W Project 1

An eBay-like auction platform built with Django where users can create listings, place bids, comment, and manage a personal watchlist.

## Demo

[![Watch the demo](https://img.shields.io/badge/YouTube-Watch%20Demo-red?logo=youtube)](https://youtu.be/ZszpgdOA6hc?si=ymGWZW4rhC6NbAae)

## Features

- **Auction listings** — create listings with a title, description, starting bid, image URL, and category
- **Active listings page** — browse all currently open auctions
- **Bidding** — place bids with validation (must exceed current highest bid and starting price)
- **Close auction** — listing owner can close the auction; highest bidder is declared the winner
- **Comments** — authenticated users can comment on any listing
- **Watchlist** — add/remove listings to a personal watchlist and view them in a dedicated page
- **Categories** — browse listings filtered by category
- **Django Admin** — site admin can manage listings, bids, and comments via the admin interface

## Tech Stack

- **Backend** — Python, Django
- **Database** — SQLite (Django ORM)
- **Templating** — Django Templates
- **Styling** — CSS, Bootstrap
- **Auth** — Django built-in authentication

## Models

| Model | Description |
|---|---|
| `User` | Extended Django AbstractUser |
| `Listing` | Auction item with title, description, price, image, category, status |
| `Bid` | Bid amount linked to a listing and a user |
| `Comment` | Text comment linked to a listing and a user |

## Project Structure

```
commerce/
├── auctions/
│   ├── templates/auctions/   # HTML templates
│   ├── static/auctions/      # CSS and static assets
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   └── admin.py
├── commerce/
│   ├── settings.py
│   └── urls.py
└── manage.py
```

## Setup

```bash
git clone https://github.com/YOUR_USERNAME/commerce.git
cd commerce
pip install -r requirements.txt
python manage.py makemigrations auctions
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

Then visit `http://127.0.0.1:8000`. Access the admin panel at `/admin`.

## Course

[CS50's Web Programming with Python and JavaScript](https://cs50.harvard.edu/web/) — Project 1

