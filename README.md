# AI Email Reply Writer - Chrome Extension

This repository contains the Chrome extension that integrates with email clients (e.g., Gmail) to add an "AI Reply" button near the send/reply button. It uses the backend API to generate replies via the Gemini AI model.

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Configuration](#configuration)
- [Installation](#installation)
- [Usage](#usage)
- [Development](#development)
- [Testing](#testing)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The extension detects email composition interfaces, injects a button, and fetches AI-generated replies from the backend when clicked. It handles email content extraction and insertion.

## Prerequisites
- Google Chrome browser
- Backend server running (from the backend repo)
- Manifest V3 compatible

## Setup
1. Clone the repository:

## Configuration
1. Update `manifest.json` with permissions if needed.
2. Create a `config.js` or use environment variables for API URLs:


## Installation
1. Open Chrome and go to `chrome://extensions/`.
2. Enable "Developer mode".
3. Click "Load unpacked" and select the extension folder.

## Usage
- Open Gmail or supported email client.
- In the reply/compose window, look for the "AI Reply" button near the send button.
- Click it to generate and insert an AI reply based on the current email thread.

## Development
- Edit content scripts (e.g., `content.js`) for DOM manipulation.
- Background scripts handle API calls.
- Reload the extension in `chrome://extensions/` after changes.

## Testing
- Test in Gmail: Compose/reply to an email and use the button.
- Debug: Use Chrome DevTools (inspect popup or content scripts).

## Deployment
- Package for Chrome Web Store:
1. Zip the extension folder.
2. Submit to [Chrome Web Store Developer Dashboard](https://chrome.google.com/webstore/devconsole).
- Ensure compliance with Chrome extension policies.

## Contributing
Fork the repo, create a feature branch, and submit a pull request. Follow Chrome extension best practices.

## License
MIT License. See [LICENSE](LICENSE) for details.
