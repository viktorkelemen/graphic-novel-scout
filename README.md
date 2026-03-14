# Graphic Novel Scout 📚

A weekly automated scanner that crawls graphic novel and comics sites, filters for literary/art comics, and delivers a curated summary via Telegram.

Runs as an [OpenClaw](https://github.com/openclaw/openclaw) cron job on a Raspberry Pi 5.

## What it does

Every Sunday at 10 AM ET, it:
1. Fetches 12 sources (review sites, publisher blogs, Reddit communities)
2. Filters for literary/art comics, graphic memoirs, translated works, political/historical non-fiction
3. Skips superhero stuff entirely
4. Cross-references against a personal reading tracker
5. Delivers a 5-10 pick summary to Telegram

## Sources

See [sources.md](sources.md) for the full list.

### News & Reviews
- The Comics Journal, Comics Beat, Broken Frontier

### Publisher Blogs
- Drawn & Quarterly, Fantagraphics

### Curated / Discovery
- Book Riot Comics, Publishers Weekly, The Nib, European Comics in Translation

### Reddit
- r/graphicnovels, r/altcomix, r/bandedessinee

## Setup

### Prerequisites
- [OpenClaw](https://github.com/openclaw/openclaw) installed and configured
- Telegram channel configured

### Install the cron job

```bash
openclaw cron add \
  --name "Weekly graphic novel scout" \
  --cron "0 10 * * 0" \
  --tz "America/New_York" \
  --session isolated \
  --message "$(cat prompt.md)" \
  --announce \
  --channel telegram \
  --to "<your-telegram-chat-id>"
```

### Test run

```bash
openclaw cron run <job-id>
```

## Files

- `prompt.md` — the agent prompt sent each run
- `sources.md` — list of scanned sources
- `cron-job.json` — exported cron job definition (for backup/restore)
