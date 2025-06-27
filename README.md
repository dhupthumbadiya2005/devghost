# DevGhost

**DevGhost** is a smart CLI tool that generates high-quality GitHub commit messages from your code diffs using Gemini AI. It streamlines your workflow, saves time, and helps you write better commit messages—automatically!

---

## 🚀 Features
- **AI-powered commit messages** from your git diff (using Gemini AI)
- **Works in any git project** (one-time setup per user)
- **Fast workflow:** Just press Enter to commit with the AI-generated message
- **Easy setup** for GitHub and Gemini API keys
- **Cross-platform:** Linux, macOS, Windows (with WSL)

---

## 📦 Installation

1. **Clone or download this repo:**
   ```sh
   git clone https://github.com/dhupthumbadiya2005/devghost.git
   cd devghost
   ```
2. **(Recommended) Create and activate a virtual environment:**
   ```sh
   python3 -m venv venv
   source venv/bin/activate
   ```
3. **Install as a CLI tool:**
   ```sh
   pip install -e .
   ```
   Or, install directly from PyPI:
   ```sh
   pip install devghost
   ```

---

## ⚙️ Setup

1. **Run the setup command to store your API keys:**
   ```sh
   devghost setup
   ```
   - **GitHub Token:** Generate a Personal Access Token (classic) with `repo` scope at [GitHub Tokens](https://github.com/settings/tokens) (set expiration up to 1 year).
   - **Gemini API Key:** Get your free API key from [Google AI Studio](https://aistudio.google.com/app/apikey)

*You only need to run setup once per user. The config is stored in your home directory (`~/.devghost`).*

---

## 🛠️ Usage

1. **Make some changes in your git project.**
2. **Run:**
   ```sh
   devghost suggest
   ```
3. **The tool will show the AI-generated commit message.**
4. **Press Enter to commit with this message, or Ctrl+C to cancel.**
   - All changes will be staged and committed automatically.

---

## 💡 Example

```sh
$ devghost suggest
Suggested commit message:
Add user authentication and update login UI
Press Enter to commit with this message, or Ctrl+C to cancel.
Committed successfully!
```

---

## ❓ FAQ

- **Do I need to run setup in every project?**
  - No, just once per user. The config is stored in your home directory (`~/.devghost`).
- **Where is my config stored?**
  - In `~/.devghost`.
- **What if I get an API error?**
  - Double-check your API keys and network connection.
- **What if I get a git error?**
  - Make sure you have changes to commit and are in a git repository.
- **How do I update my API keys?**
  - Run `devghost setup` again.

---

## 📄 License
MIT 