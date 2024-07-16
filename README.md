# Internet Speed Twitter Bot

This project is a Python script that uses Selenium to automatically check your internet speed and tweet at your internet provider if the speed is lower than expected. 

## Features

- Automatically checks your internet speed using [speedtest.net](https://www.speedtest.net)
- Compares the speed against your promised internet speed
- Logs into Twitter and tweets at your internet provider if the speed is lower than expected

## Requirements

- Python 3.x
- Selenium
- ChromeDriver (compatible with your version of Google Chrome)

## Setup

1. **Clone the repository:**

    ```sh
    git clone https://github.com/Prathamesh326/Twitter-Complaint-Bot.git
    cd Twitter-Complaint-Bot
    ```

2. **Install the required packages:**

    ```sh
    pip install selenium
    ```

3. **Download ChromeDriver:**

    Download ChromeDriver from [here](https://sites.google.com/a/chromium.org/chromedriver/downloads) and place it in the same directory as your script or add it to your PATH.

4. **Update the script with your details:**

    Open `complain.py` and update the following variables with your information:

    ```python
    PROMISED_DOWN = 150     # Change this according to your internet plan
    PROMISED_UP = 10        # Change this according to your internet plan
    TWITTER_EMAIL = "_____ENTER YOUR OWN EMAIL_____"
    TWITTER_PASSWORD = "_____ENTER YOUR OWN PASSWORD_____"
    USERNAME = "_____ENTER YOUR OWN TWITTER USERNAME_____"
    ```

## Usage

1. **Run the script:**

    ```sh
    python main.py
    ```

2. The script will:
   - Open a browser and navigate to speedtest.net
   - Perform an internet speed test
   - Log in to Twitter
   - Tweet at your internet provider if the speed is lower than expected

## Notes

- Ensure that your Twitter account has 2-factor authentication disabled for the script to log in successfully.
- Make sure your Chrome browser is updated to avoid compatibility issues with ChromeDriver.

## Contributing

Feel free to fork this repository and submit pull requests. If you find any issues, please open an issue on GitHub.
