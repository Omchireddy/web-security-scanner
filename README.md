
# Web Security Scanner Chrome Extension

The Web Security Scanner is a Chrome extension designed to help users identify potential security vulnerabilities on web pages. It scans for common threats such as Cross-Site Scripting (XSS) and SQL Injection, as well as checks for secure connections (HTTPS).


## features
- XSS Detection: Identifies potential XSS vulnerabilities using static and heuristic analysis.
- SQL Injection Detection: Scans for common SQL injection patterns.
-  Security Check: Alerts users if the page is not served over HTTPS or contains mixed content.
-  User -Friendly Interface: Simple popup interface to initiate scans and display results.

## Installation
- Open Chrome and navigate to ```chrome://extensions/``` .
- Enable ```"Developer mode"``` in the top right corner.
- Click on ```"Load unpacked"``` and select the folder containing the extension files.
- The Web Security Scanner extension should now be installed and visible in your extensions list.

## Usage
-  Click on the Web Security Scanner icon in the Chrome toolbar.
-  Click the "Scan for Vulnerabilities" button.
- The extension will scan the current web page for XSS and SQL - injection vulnerabilities, as well as check for secure connections.
- Results will be displayed in the popup interface.

## File Structure
```
MultipleFiles/

│

├── background.js      # Handles messages and executes scripts in the active tab.

├── content.js         # Contains functions to detect XSS and SQL injection vulnerabilities.

├── popup.html         # The HTML structure for the popup interface.

├── popup.js           # JavaScript for handling user interactions in the popup.
```

## Code Explanation
- ****background.js****: Listens for messages from the popup and executes scripts in the active tab to display results.
- ****content.js****: Contains the logic for detecting XSS and SQL injection vulnerabilities, as well as checking the security of the page.
- ****popup.html****: The user interface for the extension, allowing users to initiate scans and view results.
- ****popup.js****: Manages the interaction between the popup and the content script, displaying the scan results.


## License
This project is licensed under the ```MIT License``` . See the LICENSE file for more details.
