# Quote Generator

A clean, lightweight Random Quote Generator built with HTML, CSS and JavaScript.

![App Screenshot](Screenshot%202024-07-02%20145539.png)

Demo: Click the "New Quote" button to fetch an inspirational quote from the Quotable API, listen to it using your browser's speech synthesis, copy it to clipboard, or share it on Twitter.

## Features

- Fetches a random quote from the Quotable API (https://api.quotable.io)
- Read quotes aloud using the Web Speech API
- Copy quote text to clipboard with one click
- Open a pre-filled tweet with the quote
- Minimal, responsive UI (index.html, style.css)

## How it works

- index.html contains the UI structure and buttons.
- style.css styles the card and controls.
- script.js handles interactions:
  - fetches JSON from the Quotable API endpoint
  - updates the quote and author in the DOM
  - uses SpeechSynthesisUtterance to speak the quote
  - copies text to the clipboard and opens Twitter's intent URL

Note: The current fetch in script.js uses `http://api.quotable.io/random`. If you plan to deploy this project over HTTPS (GitHub Pages or similar), change that URL to `https://api.quotable.io/random` to avoid mixed-content errors.

## Installation & Usage

1. Clone or download this repository.
2. Open `index.html` in your browser (or host it on any static file server).
3. Click "New Quote" to load a random quote.
4. Use the icons to speak, copy, or tweet the quote.

## Files

- `index.html` — markup and UI
- `style.css` — styling
- `script.js` — behavior and API calls
- `Screenshot 2024-07-02 145539.png` — demo screenshot included in this repo

## Contributing

Contributions and improvements are welcome. Open an issue or send a pull request with changes.

## Notes

- Requires a modern browser with support for fetch, Clipboard API and Web Speech API.
- If speech isn't working, ensure your browser supports the Speech Synthesis API and that the page isn't muted.
