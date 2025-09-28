# n8n on Render 🚀

This repo deploys [n8n](https://n8n.io) automation server to [Render](https://render.com).

## Quick Deploy

1. Fork this repo
2. Go to [Render Dashboard](https://dashboard.render.com/)
3. Click **New → Web Service**
4. Connect your forked repo
5. Render auto-detects the `Dockerfile` and deploys

## First Run

Open `https://<your-render-subdomain>.onrender.com`  
and create your n8n admin user.

## Persistent Database (optional)

To keep workflows/settings after redeploys:
- Add a free Render **Postgres** database
- Add these env vars:

```
DB_TYPE=postgresdb
DB_POSTGRESDB_HOST=<render-host>
DB_POSTGRESDB_PORT=5432
DB_POSTGRESDB_USER=<username>
DB_POSTGRESDB_PASSWORD=<password>
DB_POSTGRESDB_DATABASE=<dbname>
```
