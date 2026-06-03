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
<img width="1693" height="1008" alt="image" src="https://github.com/user-attachments/assets/06e764f7-846e-4580-9d0e-a20772820b7b" />

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
- https://data.weather.gov.hk/weatherAPI/opendata/weather.php?dataType=flw&lang=en
  
- Hong Kong Observatory Open Data API Documentation
- https://www.hko.gov.hk/en/weatherAPI/doc/files/HKO_Open_Data_API_Documentation.pdf
  
- RTHK RSS Feeds (Local, International, Finance)
- https://rthk.hk/rthk/news/rss/e_expressnews_elocal.xml
- https://rthk.hk/rthk/news/rss/e_expressnews_einternational.xml
- https://rthk.hk/rthk/news/rss/e_expressnews_efinance.xml
  
- Telegram APIs
- https://core.telegram.org/
