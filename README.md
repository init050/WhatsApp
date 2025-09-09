# WhatsApp Message Bot

This is a Python script that automates sending WhatsApp messages to multiple contacts using Selenium.

## Project Overview

The WhatsApp Message Bot is a simple but powerful script that allows you to send a message to a list of your WhatsApp contacts multiple times. It uses Selenium to control a web browser, navigate to WhatsApp Web, and send the messages automatically.

This project is a fun example of what can be accomplished with browser automation and can be a starting point for more complex WhatsApp bots.

**Disclaimer:** This script is for educational purposes only. Automating user accounts can be against the terms of service of some platforms. Use it responsibly.

## Features

*   **Bulk messaging:** Send a message to multiple contacts at once.
*   **Message repetition:** Send the same message multiple times to each contact.
*   **Interactive input:** Prompts the user for the contact names, the message, and the number of times to send it.

## Technologies Used

*   **Language:** Python
*   **Automation Library:** [Selenium](https://www.selenium.dev/)

## Installation and Setup

To run this script, you'll need Python, pip, and Google Chrome.

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd WhatsApp
    ```

2.  **Create a virtual environment and activate it:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the dependencies:**
    ```bash
    pip install selenium
    ```

4.  **Download ChromeDriver:**
    You'll need to download the version of ChromeDriver that corresponds to your version of Google Chrome.
    *   You can download ChromeDriver from the official website: [https://chromedriver.chromium.org/downloads](https://chromedriver.chromium.org/downloads)
    *   Make sure that the `chromedriver` executable is in your system's PATH or in the same directory as the script.

## How to Use

1.  **Run the script:**
    ```bash
    python WhatsApp_bot.py
    ```

2.  **Log in to WhatsApp Web:**
    The script will open a new Chrome window and navigate to `https://web.whatsapp.com/`. You'll need to scan the QR code with your phone to log in.

3.  **Provide the inputs:**
    *   Once you're logged in, go back to the terminal where the script is running.
    *   Enter a comma-separated list of the names of the contacts you want to message (the names must match exactly how they appear in your WhatsApp contacts).
    *   Enter the message you want to send.
    *   Enter the number of times you want to send the message to each contact.
    *   Press Enter to start the bot.

The script will then find each contact and send the message the specified number of times.

**Note:** The script relies on class names from the WhatsApp Web interface, which can change over time. If the script doesn't work, you may need to update the class names in the `WhatsApp_bot.py` file.

## Future Improvements

*   **More robust element selection:** Use more stable selectors (like data attributes) instead of class names to make the script less likely to break when WhatsApp Web is updated.
*   **Error handling:** Add error handling to gracefully manage cases where a contact is not found.
*   **GUI interface:** Create a simple graphical user interface to make the bot easier to use for non-technical users.
*   **Read contacts from a file:** Allow the user to provide a list of contacts from a text file or a CSV.
