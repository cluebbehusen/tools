# UUID Generator

Generate random UUIDs (v4).

## Features

- **Single generation**: One-click UUID creation with instant copy
- **Auto-generate on load**: A fresh UUID is ready as soon as you open the page
- **Bulk generation**: Create up to 1000 UUIDs at once
- **Click to copy**: Click any UUID in the bulk list to copy it individually
- **JSON output**: Toggle to format bulk output as a JSON array
- **Copy all**: Copy the entire bulk list (newline-separated or JSON)

## Implementation

Uses the native `crypto.randomUUID()` API available in all modern browsers. No external dependencies.
