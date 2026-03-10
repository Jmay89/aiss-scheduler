# aiss-scheduler

> GitHub Actions cron scheduler for MedSiteAI — triggers scheduled post publishing every 15 minutes.

## Tech Stack
| Dep | Purpose |
|-----|---------|
| GitHub Actions | Cron-based workflow |

## Architecture
- **Entry point**: `.github/workflows/` (GitHub Actions YAML)
- **Design pattern**: Scheduled HTTP trigger → Vercel endpoint
- **Data flow**: Cron fires → hits APP_URL/api/publish-scheduled → posts go live

## Key Files
| File | Purpose |
|------|---------|
| `README.md` | Setup instructions |
| `.github/workflows/` | Cron workflow definitions |

## Environment
- `APP_URL` — Vercel app URL (e.g., `https://aiss-builder.vercel.app`)
- `CRON_SECRET` — Auth key for the cron endpoint

## How to Run
Runs automatically via GitHub Actions every 15 minutes. Manual trigger available in Actions tab.
