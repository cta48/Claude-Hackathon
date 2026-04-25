# Decision Clarity 🧠

> An AI-powered tool that helps people think through decisions more clearly — without telling them what to do.

Built for the **Claude Builder Club Hackathon 2026** | Focus area: **Neuroscience & Mental Health**

---

## What it does

Instead of giving advice, Decision Clarity breaks down any decision into 3 honest perspectives:

| Perspective | Description |
|---|---|
| 👍 **Best Case** | What's the ideal outcome if things go well |
| ⚖️ **Likely Outcome** | What will realistically probably happen |
| 💥 **Worst Case** | What could go wrong |

The goal is to expand access to structured thinking — the kind of perspective-taking that therapists and coaches use — for anyone facing a hard decision.

---

## Demo

👉 **[Live App](https://cta48.github.io/Claude-Hackathon/)**

---

## Tech Stack

- **Frontend:** Vanilla HTML, CSS, JavaScript (no frameworks)
- **AI:** Anthropic Claude API (`claude-sonnet-4-20250514`)
- **Hosting:** GitHub Pages

---

## Setup Instructions

### 1. Clone the repo
```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
```

### 2. Get an Anthropic API key
- Go to [console.anthropic.com](https://console.anthropic.com)
- Create a new API key

### 3. Add your API key
Open `index.html` and find this line near the bottom:
```js
const API_KEY = 'YOUR_API_KEY_HERE';
```
Replace `YOUR_API_KEY_HERE` with your actual key.

### 4. Run locally
Just open `index.html` in your browser — no build step needed.

### 5. Deploy to GitHub Pages
- Push your code to GitHub
- Go to repo **Settings → Pages**
- Set source to **Deploy from a branch → main → / (root)**
- Your app will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME`

---

## Challenges

- **API key security:** Direct browser access to the Anthropic API exposes the key in client-side code. For a production app, this would be handled via a backend proxy. For this hackathon demo, we use Anthropic's `anthropic-dangerous-direct-browser-access` header which is intended for prototyping.
- **Structured output:** Getting Claude to consistently return valid JSON required a carefully written system prompt with explicit formatting instructions and error handling for edge cases.

---

## Social Impact

Poor decision-making costs people relationships, money, and mental health. Structured thinking frameworks (like pre-mortems and scenario planning) are well-documented tools — but most people don't have access to a coach or therapist to guide them through one. This tool makes that kind of structured reflection freely available to anyone.

---

## Team

- Christopher Au, Bao PHam (https://github.com/cta48)
