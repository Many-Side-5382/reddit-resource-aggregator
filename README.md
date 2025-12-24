# Reddit Read-Only Research Collector (Personal Use)

## Purpose
A non-commercial, read-only tool that collects public Reddit threads and comment trees to produce non-identifying, aggregated summaries (e.g., common themes, frequently recommended resources).

## Scope (initial)
- Subreddits: r/CompTIA, r/WGUCyberSecurity, r/WGU
- Time window: configurable (e.g., last 6 months)
- Topic filtering: configurable keywords (e.g., PenTest+ PT0-003 variants)

## What it does
- Searches within the approved subreddits for matching topics
- Fetches the thread content and the full comment tree (when available via the API)
- Exports machine-readable JSONL for offline analysis

## What it does NOT do
- No posting, commenting, voting, messaging, or moderation actions
- No circumvention of rate limits or access controls
- No attempt to identify or profile users
- No AI/ML/LLM training or fine-tuning

## Rate limiting & compliance
- Uses OAuth via Reddit’s Data API
- Uses a descriptive User-Agent
- Throttles requests and backs off on 429s
- Stores data locally for analysis only; no public dataset distribution

## Data handling
- Output files are not committed to this repo
- Credentials are provided via environment variables (never committed)
