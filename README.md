# AI Morning Markets Brief

![Morning Markets Brief Preview](preview.png)

> Automated AI workflow that fetches live financial news every morning, analyzes it with Groq AI, and delivers a beautiful digest to your inbox — zero manual effort.

---

## What it does

1. **Fetches** live news from Bloomberg, Reuters and Yahoo Finance RSS feeds
2. **Analyzes** headlines with Groq AI (Llama 3.1) to extract key insights
3. **Delivers** a formatted HTML email digest automatically every morning

## What the email contains

- Overall market sentiment — Bullish / Bearish / Neutral
- 3 top investment themes with supporting articles
- Key tickers in the news
- Market summary paragraph
- Watch list for the day
- Contrarian take on the news

## Stack

- **n8n** — visual workflow automation
- **Groq API + Llama 3.1** — AI analysis
- **Bloomberg / Reuters / Yahoo Finance** — RSS feeds
- **Gmail SMTP** — email delivery

## Setup

### 1. Import workflow
- Open n8n at `localhost:5678`
- Click **Import** and upload `workflow.json`

### 2. Add your Groq API key
- Get a free key at [console.groq.com](https://console.groq.com)
- Open the **Groq AI Analysis** node
- Replace `gsk_your_key_here` with your actual key

### 3. Add Gmail credentials
- Open the **Send Email** node
- Enter your Gmail address and [App Password](https://myaccount.google.com/apppasswords)

### 4. Activate
- Click the **Activate** toggle in the top right
- Workflow runs automatically every morning at 6 AM

## Built with

Built in one afternoon as a demonstration of AI workflow automation
for financial news aggregation and summarization.
