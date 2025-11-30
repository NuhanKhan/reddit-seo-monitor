# reddit-seo-monitor

Personal-use n8n workflow that checks a small set of SEO-related subreddits once per day and sends a concise summary to my personal WhatsApp.

- Runs: daily (cron)
- Subreddits monitored: r/SEO, r/bigseo, r/TechSEO, r/digital_marketing
- Max posts fetched: 20 per subreddit per run (configurable)
- Auth: OAuth2 Authorization Code (user consent required)
- Data handling: **All Reddit data is deleted immediately after the daily summary is generated.**

## Files
- workflow/reddit-seo-workflow.json — n8n importable workflow
- privacy.md — privacy statement

## How to use
1. Import workflow into n8n.
2. Create OAuth2 Reddit credential (Authorization Code) and set credential in the Reddit Search node.
3. Set environment variables for WhatsApp / OpenAI credentials.
