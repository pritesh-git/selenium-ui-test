# Selenium Web Automation Script

This Python script uses Selenium WebDriver to automate interactions with a specific web page (http://demo.automationtesting.in/). It performs various actions, including login, registration, alert handling, and interactions with iframes.

## Project Overview

This project demonstrates the use of Selenium for web automation, focusing on:

* Automated login and registration processes.
* Handling different types of JavaScript alerts (accept, dismiss, send keys).
* Switching contexts to interact with iframes.
* Simulating user scrolling.
* Basic browser setup and control.

## Technologies Used

* **Python:** 3.x
* **Selenium WebDriver:** For browser automation.
* **ChromeDriver:** For controlling the Google Chrome browser.

## Prerequisites

* **Python:** Ensure Python 3.x is installed on your system.
* **Selenium:** Install the Selenium library using pip:

    ```bash
    pip install selenium
    ```

* **ChromeDriver:**
    * Download the ChromeDriver executable that corresponds to your Chrome browser version from the official ChromeDriver website.
    * Place the ChromeDriver executable in a directory that is in your system's PATH environment variable, or specify the path directly in the script.

## Getting Started

1.  **Clone the Repository (if applicable):**

    ```bash
    git clone <repository_url>
    cd <repository_directory>
    ```

2.  **Install Dependencies:**

    ```bash
    pip install selenium
    ```

3.  **Configure ChromeDriver:**
    * Ensure that the `driver_location` variable in the script points to the correct location of your ChromeDriver executable.
    * Ensure that the `binary_location` variable points to the location of your Chrome binary.

4.  **Run the Script:**

    ```bash
    python <script_name>.py
    ```

    Replace `<script_name>.py` with the actual name of your Python script.

## Script Description

* **Import Statements:** The script imports necessary modules from Selenium, time, and os.
* **Driver Setup:**
    * Configures Chrome options (window size, position, incognito mode).
    * Initializes the Chrome WebDriver.
    * Navigates to the target URL.
* **Function Calls:**
    * `loginScreen(driver, sleep)`: Simulates a login action.
    * `registerScreen(driver, Select, os)`: Fills out a registration form.
    * `switchToAlert(driver, sleep)`: Handles various JavaScript alert types.
    * `switchToIframe(driver, sleep)`: Switches to and interacts with iframes.
* **Scrolling:** Simulates scrolling down the page.
* **Browser Closure:** Closes the browser window.
* **Defined functions:**
    * `switchToAlert()`: Handles Javascript alert boxes.
    * `switchToIframe()`: Handles Iframe switching.
    * `loginScreen()`: Handles login functionality.
    * `registerScreen()`: Handles registration functionality.

## Notes

* Ensure your ChromeDriver version is compatible with your Chrome browser version.
* Adjust the script's locators (XPath, ID, etc.) if the target website's structure changes.
* The script uses `time.sleep()` for demonstration purposes. In a production environment, consider using explicit or implicit waits for better reliability.
* The script assumes the existence of `loginScreen.py`, `registerScreen.py`, and `switchTo_menu.py` files. Ensure these files are present in the same directory as the main script.

## Contributing

Feel free to contribute to this project by submitting pull requests.

## License

This project is open-source and available under the MIT License.
