# Community Bot
## Overview
Welcome to the Community Bot repository! This bot automates the process of following back users who follow you and unfollowing those who unfollow you on GitHub.

## Key Features
### Automatic Follow Back: 
You can follow-back users automatically just by running the script followback.js! 😊
### Automatic Unfollow: 
You can unfollow users automatically who don't follow you back. 😁
### Scheduled Runs: 
The repository includes scheduling this automated behaviour on GitHub Actions

## Important Notes
### Respect: 
The bot follows and unfollows based on a simple rule: if you follow me, I’ll follow you back; if you unfollow me, I’ll unfollow you. It’s all automated, so please be mindful of this automatic process.
### GitHub’s Rate Limits: 
Please note that GitHub has rate limits on API calls. The bot will respect these limits, but excessive use may temporarily block requests.

## How to Use

### Clone the repository:
git clone https://github.com/yourusername/community-bot.git <br>
cd community-bot

### Set Up the Bot: Create a .env file with your GitHub username and token:
GITHUB_USERNAME=your_github_username     <br>
GITHUB_TOKEN=your_github_token

### Install Dependencies: Install the necessary packages (axios and dotenv):
npm install axios dotenv

### Run the Bot: Run the bot to follow or unfollow users:
node followback.js

### Running Automatically (via GitHub Actions)
Set up your GitHub Secrets for GITHUB_USERNAME and GITHUB_TOKEN.     <br>
The bot will run automatically based on the schedule defined in .github/workflows/follow-back.yml.

## License
This repository is licensed under the MIT License. See LICENSE for more details.
