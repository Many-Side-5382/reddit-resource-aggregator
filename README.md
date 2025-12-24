# Read-only Reddit Research Collector (Personal Use)

## Purpose
Non-commercial, read-only tool to collect public Reddit posts and comment trees and produce aggregated, non-identifying summaries (e.g., common themes and frequently recommended resources).

## Initial scope
- Subreddits: r/CompTIA, r/WGUCyberSecurity, r/WGU
- Time window: configurable (e.g., last 6 months)
- Topics: configurable (e.g., PenTest+ PT0-003 and other tech/cert topics)

## What it does
- Searches within the approved subreddits for matching topics
- Fetches thread content and comment trees for offline analysis
- Exports machine-readable outputs (e.g., JSONL)

## What it does NOT do
- No posting, commenting, voting, messaging, or moderation actions
- No attempts to bypass rate limits or access controls
- No re-identification or user profiling
- No AI/ML/LLM training or fine-tuning
- No redistribution of raw datasets

## Rate limiting & compliance
- Uses OAuth and a descriptive User-Agent
- Throttles requests and backs off on rate-limit responses (e.g., HTTP 429)
- Stores data locally for analysis only; output files are not committed to this repo

## Data handling
- Credentials are supplied via environment variables (never committed)
- Output/data files are intentionally excluded via .gitignore

## Scope changes & retention
- This tool is intended for read-only, non-commercial analysis. If scope expands materially (e.g., many additional subreddits), it will be updated through the approval process before expansion.
- Stored data is kept only as long as needed for analysis; output datasets are not published.

## Notes
This repository is intentionally minimal for review/approval. It does not contain collected datasets or credentials.
