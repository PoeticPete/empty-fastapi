# Hello World FastAPI

## Installation

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Run

```bash
uvicorn main:app --reload
```

## Usage

Visit `http://127.0.0.1:8000/ping` to see the response.

## Production

To run in production, use `gunicorn` with `uvicorn` workers:

```bash
gunicorn -w 4 -k uvicorn.workers.UvicornWorker main:app
```
