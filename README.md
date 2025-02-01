# Discord Auto Chat

Discord bot for auto-leveling with auto-messaging feature that supports multiple accounts.

## Features

- Support multiple accounts (tokens)
- Auto delete messages after sending
- Channel timeout detection
- Rate limit and slowmode handling
- Complete error handling
- Customizable delay between messages
- 54 random message variations

## Requirements

- Python 3.7+
- discord.py 1.7.3
- asyncio
- colorama

## Installation 

1. Clone this repository
```bash
git clone https://github.com/Idevxd/dc.git
cd dc
```

2. Setup Virtual Environment
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Linux/Mac
python3 -m venv venv
source venv/bin/activate
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

## Usage

1. Create a `token.txt` file and enter the Discord tokens (one token per line)
```
TOKEN1
TOKEN2
TOKEN3
```

2. Run The Script
```bash
python3 jawa.py
```

3. Enter the requested information:
- Channel ID
- Number of messages to send
- Delay between each message (in seconds)

## How yo get Discord Token

1. Open Discord in a browser
2. Press F12 to open Developer Tools
3. Go to the Network tab
4. Type "api" in the filter
5. Find requests that have the "authorization" header
6. Copy the token value from there

## How to get Channel ID

1. Enable Developer Mode in Discord (User Settings > App Settings > Advanced > Developer Mode)
2. Right-click on the channel
3. Select "Copy ID"

## Warning 

⚠️ **Important**:
- Using self-bots violates Discord's Terms of Service
- Use at your own risk
- A minimum delay of 10 seconds between messages is recommended
- Make sure the token used is valid and fresh

## Error Handling

The script will handle various types of errors:
- Invalid/expired token
- Channel not found
- Channel timeout
- Rate limit
- Slowmode
- No permission to send/delete messages
- Voice channel detection

## Usage Tips

1. Use a safe delay:
- Minimum 10 seconds between messages
- Do not spam too many messages

2. If an error occurs:
- Invalid token: Update the token in token.txt
- Rate limit: The script will automatically wait
- Timeout: Wait until the timeout is complete

