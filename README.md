# sheets-to-telegram-bot-alerts
A Make.com automation blueprint that watches a Google Sheet for new row entries and automatically dispatches real-time message updates via a Telegram Bot.
# Google Sheets to Telegram Bot Alert Automation

This repository contains a Make.com (formerly Integromat) scenario blueprint that connects a Google Sheets data source to a Telegram Bot for automated, real-time message broadcasting.

## 🚀 How It Works
1. **Trigger (Google Sheets - Watch New Rows):** Monitors a specific spreadsheet on a set polling interval to capture newly appended row entries.
2. **Action (Telegram Bot - Send a Text Message or a Reply):** Automatically processes the incoming row variables, structures the message content, and pushes it directly into a specific Telegram chat, channel, or group via a custom bot.

## 📦 What's Included
* `/blueprints/sheets-to-telegram-bot-alerts.json`: The complete exported Make.com scenario configuration file.

## 🔧 Setup Instructions
1. Open your **Make.com** dashboard.
2. Create a new scenario, click the three dots (`...`) located on the bottom navigation bar, and click **Import Blueprint**.
3. Upload the `.json` blueprint file from this repository.
4. Establish your account connections:
   * **Google Sheets Module:** Connect your Google account and select your targeted spreadsheet and data sheet tab.
   * **Telegram Bot Module:** Generate an API Token from Telegram's `@BotFather`, create a new connection in Make using that token, and specify the destination `Chat ID`.
5. Map the desired column data values dynamically into your Telegram text body.
6. Save the configuration and flip the main scheduling toggle switch to **ON**.
