# Password Generator

Generate cryptographically secure random passwords.

## Features

- **Customizable length**: Choose password length from 4 to 64 characters
- **Character type selection**: Mix lowercase, uppercase, numbers, and symbols
- **Strength indicator**: Real-time entropy calculation shows password strength
- **One-click copy**: Copy generated passwords to clipboard instantly
- **Remembers your picks**: Length and character type preferences persist via local storage
- **Auto-generate on load**: A strong password is ready when you open the page using your saved settings

## Security

Uses the Web Crypto API (`crypto.getRandomValues()`) for cryptographically secure random number generation. This is suitable for password generation and much more secure than `Math.random()`. All processing happens entirely in your browser—passwords are never sent over the network.

## Implementation

Pure HTML, CSS, and vanilla JavaScript with no external dependencies. Uses native browser cryptography APIs available in all modern browsers.
