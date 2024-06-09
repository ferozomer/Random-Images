# Random Image

This project is a Telegram bot designed to handle images sent to a specific Telegram group. It downloads, stores, and serves images through an Express server. Additionally, it provides routes to fetch images and serve a random image from the stored collection.

## Project Overview

**Purpose:**  
The primary purpose of this project is to automate the handling of images sent to a designated Telegram group. The bot will download the images, store them locally, and provide a web interface to access these images.

**Target Audience:**  
This bot is intended for developers and Telegram group administrators who want an automated solution to manage images shared in their groups.

**Key Features:**
- Downloads and stores images sent to a specific Telegram group.
- Serves stored images via an Express web server.
- Provides an endpoint to serve a random image from the stored collection.
- Ensures that only one instance of the bot runs at a time.

## Installation Instructions

### Prerequisites
- Node.js (version 12 or higher)
- npm (Node package manager)

### Steps to Set Up the Project

1. **Clone the repository:**
    ```bash
    git clone https://github.com/ferozomer/Telegram-Random-Image-Bot
    cd Telegram-Random-Image-Bot
    ```

2. **Install dependencies:**
    ```bash
    npm install
    ```

3. **Set up environment variables:**
    Create a `.env` file in the root directory of the project and add the following variables:
    ```plaintext
    TELEGRAM_TOKEN=your_telegram_bot_token
    GROUP_ID=your_telegram_group_id
    ```

4. **Run the bot and Express server:**
    ```bash
    node index.js
    ```

## Usage Guide

### Starting the Application

To start the application, run the following command in the project directory:
```bash
node index.js
```

### Basic Usage

- **Sending Images:**
  Send images to the designated Telegram group. The bot will automatically download and store these images.

- **Accessing Images:**
  - To view a specific image, navigate to: `http://localhost:5000/images/<filename>`
  - To view a random image, navigate to: `http://localhost:5000/random-image`

### Health Check

To check if the server is running, navigate to:
```plaintext
http://localhost:5000/health
```

## Configuration

The application requires the following configuration through environment variables:

- `TELEGRAM_TOKEN`: The token for your Telegram bot.
- `GROUP_ID`: The ID of the Telegram group where the bot will listen for images.

Example `.env` file:
```plaintext
TELEGRAM_TOKEN=your_telegram_bot_token
GROUP_ID=your_telegram_group_id
```

## Contributing

### Submitting Issues

If you encounter any issues, please submit them through the GitHub repository's issues page. Provide a detailed description of the problem, steps to reproduce, and any relevant logs or screenshots.

### Proposing Enhancements

We welcome enhancements and new features. If you have an idea, please open a discussion in the issues page or submit a pull request with your proposed changes.

### Pull Requests

To submit a pull request:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes with clear and descriptive messages.
4. Push your branch to your forked repository.
5. Open a pull request against the main branch of the original repository.

## License Information

This project is licensed under the MIT License. You are free to use, modify, and distribute this software, provided that you include the original license and copyright notice in any substantial portions of the software.

For more details, refer to the [LICENSE](LICENSE) file.

---

Thank you for using the Telegram Image Bot. We hope it serves your needs effectively. Happy coding!
