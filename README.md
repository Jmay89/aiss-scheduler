# AISS Scheduler

Cron jobs for AISS Builder - triggers scheduled post publishing every 15 minutes.

## Setup

Add these secrets in **Settings → Secrets → Actions**:

| Secret | Value |
|--------|-------|
| `APP_URL` | Your Vercel app URL (e.g., `https://aiss-builder.vercel.app`) |
| `CRON_SECRET` | The secret key your cron endpoint expects |

## Manual Trigger

Go to **Actions** → **Publish Scheduled Posts** → **Run workflow**
