# HongKong_MorningBriefing_n8n
Automated HK morning briefing with weather and news via n8n

# 🌅 HK Morning Briefing - n8n Workflow

Automated daily briefing for Hong Kong residents covering 
weather, local, international and finance news via AI.

## Features
- 🌤️ Live HK weather + temperature data
- 📰 AI-selected top 2 stories from 3 RSS feeds
- 🤖 AI-generated personalised briefing
- 📱 Delivered via Telegram

## Workflow Structure
Schedule Trigger → Weather + RSS feeds → AI filtering 
→ Merge → Final AI Agent → Telegram

## How to Use
1. Import the .json file into your n8n instance
2. Set up your credentials:
   - Anthropic API key (for AI nodes)
   - Telegram Bot token + Chat ID
3. Activate the workflow

## Nodes Required
- HTTP Request
- RSS Read
- AI Agent (Claude)
- Code
- Merge
- Telegram

## Data Sources
- HK Observatory Weather API
- RTHK RSS Feeds (Local, International, Finance)
