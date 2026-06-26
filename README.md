# ProductHub API

A backend service built with FastAPI and PostgreSQL for browsing a large product catalog. This project was developed as part of the CodeVector Internship Take-Home Task.

## Features

- Browse 200,000+ products
- Newest-first sorting
- Filter by category
- Fast cursor-based pagination
- PostgreSQL database
- Bulk product seed script
- REST API with Swagger documentation

## Tech Stack

- Python 3
- FastAPI
- SQLAlchemy
- PostgreSQL (Neon)
- Faker
- Uvicorn

## Project Structure

```
producthub-api/
├── app/
├── seed.py
├── requirements.txt
├── .env
└── README.md
```

## Installation

```bash
git clone <repository-url>
cd producthub-api

python -m venv venv
venv\Scripts\activate   # Windows

pip install -r requirements.txt
```

## Run the Project

```bash
uvicorn app.main:app --reload
```

Open:

```
http://127.0.0.1:8000/docs
```

## Database

- PostgreSQL (Neon)
- 200,000 fake products generated using Faker

## API Endpoints

- `GET /products` – Get products
- `GET /products?category=Electronics` – Filter by category
- `GET /products?limit=20` – Limit results
- `GET /products?cursor=<cursor>` – Cursor pagination

## Author

**Gokul**
