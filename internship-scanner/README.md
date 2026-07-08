# 🔍 Internship Opportunity Scanner

Automatically scans Internshala every 2 hours and sends 
real-time alerts to a Telegram group.

## 📸 Preview
[Add your Telegram screenshot here]

## ⚙️ How It Works
1. Schedule Trigger fires every 2 hours
2. HTTP Request fetches Internshala listings
3. HTML node extracts job title, company, stipend
4. Code node formats top 2 results
5. Telegram bot sends alert to group

## 🔧 Setup Instructions
1. Import `workflow.json` into your n8n
2. Create a Telegram bot via @BotFather
3. Get your Chat ID or Group ID
4. Add credentials in n8n
5. Activate workflow!

## 📊 Workflow Nodes
| Node | Purpose |
|---|---|
| Schedule Trigger | Runs every 2 hours |
| HTTP Request | Fetches Internshala page |
| HTML Extract | Pulls job details |
| Code (JS) | Formats message |
| Telegram | Sends alert |

## 💬 Sample Alert
```
🔥 New Internship Alert!
💼 Role: Python Developer
🏢 Company: SaasBanana Technologies  
💰 Stipend: ₹8,000/month
🔗 internshala.com/internships

⚡ Apply before others do!
```
