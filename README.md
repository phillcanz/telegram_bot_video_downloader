
# Telegram Video Downloader Bot

This is a Telegram bot that downloads videos from provided URLs and sends them back to the user. The bot supports various video platforms including Instagram posts and stories.

## Features

- Download videos from URLs
- Send downloaded videos to the user on Telegram
- Supports various video platforms including Instagram

## Setup

### Prerequisites

- Python 3.9 or higher
- Docker (optional, for containerized deployment)

### Installation

1. **Clone the repository**:

    ```bash
    git clone https://github.com/yourusername/telegram-video-downloader-bot.git
    cd telegram-video-downloader-bot
    ```

2. **Create a `.env` file**:

    Create a `.env` file in the root of the project directory and add your Telegram bot token:

    ```
    TELEGRAM_BOT_TOKEN=your_bot_token_here
    ```

3. **Install dependencies**:

    If you're running the bot locally, install the required Python packages:

    ```bash
    pip install -r requirements.txt
    ```

4. **Run the bot**:

    ```bash
    python bot_script.py
    ```

### Using Docker

To run the bot in a Docker container, follow these steps:

1. **Build the Docker image**:

    ```bash
    docker build -t telegram-video-bot:v1.0.0 .
    ```

2. **Run the Docker container**:

    ```bash
    docker run -d --name telegram-video-bot-v1.0.0 --env-file .env telegram-video-bot:v1.0.0
    ```

### Notes

- Ensure that the `.env` file is listed in your `.gitignore` file to prevent it from being tracked by version control.
- The `.env` file should contain your Telegram bot token as shown above.

### Example `.gitignore`

```
# .gitignore
.env
```

### Project Structure

```
telegram-video-downloader-bot/
├── bot_script.py
├── Dockerfile
├── requirements.txt
├── .env
└── .gitignore
```

### Environment Variables

- `TELEGRAM_BOT_TOKEN`: Your Telegram bot token obtained from BotFather.

### Contributing

Feel free to open issues or submit pull requests with improvements. Make sure to follow the project's code of conduct.

### License

This project is licensed under the MIT License.
