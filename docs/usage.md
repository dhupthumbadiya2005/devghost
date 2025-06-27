# Usage Guide

## Setup

Run the setup command once to store your API keys:

```sh
devghost setup
```
- Enter your GitHub Personal Access Token (classic, repo scope, 1 year expiry recommended)
- Enter your Gemini API Key

## Generate a Commit Message

1. Make changes in your git project.
2. Run:
   ```sh
   devghost suggest
   ```
3. The tool will show the AI-generated commit message.
4. Press Enter to commit, or Ctrl+C to cancel.

## Advanced
- Works with any git project.
- Only needs setup once per user.
- Supports all platforms (Linux, macOS, Windows with WSL). 