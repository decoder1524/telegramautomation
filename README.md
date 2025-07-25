﻿# telegramautomation

This project allows you to automate two major tasks on Telegram:

1. **Scrape members** from any group you're part of.
2. **Add members** from a CSV file to a chosen Telegram group.

Built with Python using the [Telethon](https://docs.telethon.dev/) library.

---

## Features

- Scrapes all members from a selected group and saves to CSV
- Adds members from CSV into another group (by username or ID)
- Uses random sleep to reduce the risk of Telegram ban
- Handles common Telegram API errors like flood limits and privacy restrictions
- Fully interactive terminal-based UI

---

## Requirements

- Python 3.7 or higher
- Telegram API credentials (get from [https://my.telegram.org](https://my.telegram.org))
- The following Python libraries:
  - `telethon`
Install them via:

```bash
pip install telethon



---

Usage

1. Clone the repository

git clone https://github.com/yourusername/telegram-group-automation.git
cd telegram-group-automation

2. Run the script

python addMembers.py

3. Follow the prompts:

Option 1: Scrape users from a group → Outputs to a CSV file

Option 2: Add users to a group → Input: CSV file

Option 3: Show users from CSV



---

📝 CSV Format

Make sure your input CSV file has the following structure (no header):

username,user_id,access_hash

Example:

john_doe,123456789,9876543210123456789


---

🛑 Warning

Adding too many users too quickly can cause Telegram to block your account temporarily.

Respect user privacy and Telegram's Terms of Service.

Use proxies or rotate accounts for high-volume tasks.

