# Discord Bot

A simple Discord bot that responds to user commands and fetches memes.

## Features

- `$hello` - Bot responds with "Hello World!"
- `$meme` - Bot sends a random meme from the meme API

## Requirements

- Python 3.8+
- discord.py
- python-dotenv
- requests

## Setup

### 1. Install Dependencies
```bash
pip install discord.py python-dotenv requests
```

### 2. Create a `.env` File
Create a `.env` file in the project root and add your Discord bot token:
```
DISCORD_TOKEN=your_discord_token_here
```

### 3. Run the Bot
```bash
python bot.py
```

## Getting Your Discord Token

1. Go to [Discord Developer Portal](https://discord.com/developers/applications)
2. Click "New Application" and give it a name
3. Go to the "Bot" tab and click "Add Bot"
4. Copy the token and paste it in your `.env` file
5. Under "OAuth2" → "URL Generator", select:
   - Scopes: `bot`
   - Permissions: `Send Messages`, `Read Messages/View Channels`
6. Use the generated URL to invite the bot to your server

## Usage

Once the bot is running and invited to your Discord server:
- Type `$hello` in any channel to get a greeting
- Type `$meme` to receive a random meme

## Notes

- Keep your `.env` file private and never commit it to GitHub
- The bot requires message content intent to read commands
