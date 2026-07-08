# 🔍 Internship Opportunity Scanner

Automatically scans Internshala every 2 hours and sends 
alerts to a Telegram group.

## What it does
- Scrapes 600+ internships from Internshala
- Filters by skills: Java, Python, JavaScript, Web Dev
- Sends top 2 new internships to Telegram group
- Runs automatically every 2 hours

## Tech Stack
- n8n (workflow automation)
- Telegram Bot API
- HTML scraping
- JavaScript

## How to use
1. Import the JSON file into your n8n instance
2. Set up your Telegram bot credentials
3. Update the Chat ID to your group
4. Activate the workflow!

## Workflow
```
[Schedule Trigger - 2hrs]
        ↓
[HTTP Request - Internshala]
        ↓
[HTML Extract - jobs]
        ↓
[Code - format message]
        ↓
[Telegram - send alert]
```
