# AI Project Tracker

Task tracker with a Telegram bot, web dashboard and a local LLM.

Runs locally with Qwen 2.5 via llama.cpp — no external API required.

## Stack

* FastAPI / SQLAlchemy
* Next.js / TypeScript / Tailwind
* Aiogram 3
* PostgreSQL / Redis
* llama.cpp / Qwen 2.5
* Docker Compose / Caddy

## Run

```bash
git clone https://github.com/vlimkv/ai-project-tracker.git
cd ai-project-tracker

cp .env.example .env
docker compose up -d --build
```

The model is downloaded on the first run.

## Access

* Web: http://localhost:3000
* API: http://localhost:8000/docs
* LLM: http://localhost:8080/v1

## Environment

```text
AI_PROVIDER=oss
OSS_MODEL=qwen2.5-3b-instruct
REDIS_URL=...
```

Requires Docker and at least 4 GB RAM. GPU is optional.
