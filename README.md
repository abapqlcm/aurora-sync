# AuroraSync

A lightweight data synchronization service built with FastAPI. It provides a simple web dashboard for managing sync channels and relay endpoints, useful for keeping distributed clients in sync across networks.

## Features

- Web-based management dashboard (dark/light mode, EN/FA)
- Create and manage sync channels with usage limits and expiry
- Per-channel traffic statistics and connection monitoring
- Subscription export for bulk configuration
- Secure token-based authentication
- Keep-alive task to stay responsive on free-tier hosts

## Quick Start (Wasmer Edge)

1. Fork this repository
2. Install the CLI: `curl https://get.wasmer.io -sSfL | sh` then `wasmer login`
3. From the repo root run: `wasmer deploy`
4. Open `https://<app-name>-<owner>.wasmer.app/login` (default password: `admin`)

## Quick Start (Render)

1. Fork this repository
2. Go to [render.com](https://render.com) and sign in with GitHub
3. Create a new **Web Service** from this repo
4. Build command: `pip install -r requirements.txt`
5. Start command: `python src/main.py`
6. Deploy and open the provided URL `/login` (default password: `admin`)

## Quick Start (Railway)

1. Fork this repository
2. Go to [railway.com](https://railway.com) and deploy from GitHub
3. Set region to Amsterdam for lower latency
4. Open the provided URL `/login`

## Configuration

| Variable | Description | Default |
|----------|-------------|---------|
| `ADMIN_PASSWORD` | Dashboard password | `admin` |
| `SECRET_KEY` | Session signing secret | auto-generated |
| `PORT` | Listen port | `8000` |

## License

MIT
