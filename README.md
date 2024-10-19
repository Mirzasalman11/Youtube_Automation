# YouTube Automation

This project automates the process of playing and replaying YouTube videos, muting them, and skipping ads using Selenium WebDriver and multiprocessing.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Future Improvements](#future-improvements)
- [License](#license)
- [Contact](#contact)

## Introduction
This Python script automates YouTube video playback by:
- Clicking "Accept All" on the YouTube homepage consent popup.
- Skipping ads if available.
- Muting the video during playback.
- Setting the playback rate to 16x.
- Continuously replaying the video when it finishes.

It uses `multiprocessing` to handle multiple videos simultaneously.

## Features
- Automates interactions with YouTube videos (skipping ads, muting, and replaying).
- Mutes videos and speeds up playback.
- Runs multiple processes for handling multiple videos in parallel.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Mirzasalman11/Youtube_Automation.git
    cd Youtube_Automation
    ```

2. Install the required dependencies:
    ```bash
    pip install multiprocess
    pip install selenium
    pip install webdriver_manager
    ```

3. Make sure you have the latest version of Chrome installed, as the script automatically manages the `chromedriver` using `webdriver_manager`.

## Usage

1. Run the script:
    ```bash
    python client.py
    ```

2. The script will prompt you to input a YouTube channel URL:
    ```bash
    Please provide channel url: <Enter the URL of the YouTube channel here>
    ```

3. The script will:
    - Fetch video links from the provided YouTube channel.
    - Open each video link in a separate browser window.
    - Click "Accept All" on the consent popup.
    - Skip ads, if present.
    - Mute the video.
    - Set the playback rate to 16x.
    - Replay the video continuously.

4. By default, it processes the first 4 video links, but you can change the limit by editing the following line in the code:
    ```python
    for link in links[:4]:
    ```

## Future Improvements
- Implement advanced error handling for slow networks or ad variations.
- Add more customization options (e.g., number of videos to open).
- Enhance the overall user experience with a better interface or logging.

## License
Specify the license under which your project is distributed (e.g., MIT License).

## Contact
Author: Mirza Salman  
Email: [salmansaluu661@gmail.com](mailto:salmansaluu661@gmail.com)  

For more details, check the repository at [YouTube Automation on GitHub](https://github.com/Mirzasalman11/Youtube_Automation).
