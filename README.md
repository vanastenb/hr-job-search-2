# 🔍 HR Job Search Agent — St. Petersburg, FL

An AI-powered job search agent built with the **Anthropic Claude API** that searches for Human Resources positions in and around St. Petersburg, Florida.

## Features
- 🤖 AI agent uses live web search to find current HR job listings
- 📍 Focused on St. Petersburg, FL and surrounding areas (Tampa Bay region)
- 💬 Conversational interface — refine searches with natural language
- 📋 Structured results with job title, company, location, and description
- 🔗 Direct links to apply

## Tech Stack
- **Frontend**: React (single-file, runs in browser)
- **AI**: Anthropic Claude API (`claude-sonnet-4-20250514`) with web search tool
- **Deployment**: GitHub Pages or any static host

## Setup

### 1. Clone the repo
```bash
git clone https://github.com/YOUR_USERNAME/hr-job-search-agent.git
cd hr-job-search-agent
```

### 2. Get your Anthropic API Key
- Sign up at [console.anthropic.com](https://console.anthropic.com)
- Create an API key under **API Keys**

### 3. Run locally
Open `index.html` in a browser, or serve with:
```bash
npx serve .
```

When prompted, enter your Anthropic API key (stored only in your browser session).

## How It Works

The agent uses Claude's **web search tool** to:
1. Search job boards (Indeed, LinkedIn, Glassdoor, etc.) for HR roles
2. Parse and structure the results
3. Respond to follow-up questions like "show me remote options" or "filter by salary over $50k"

## Example Queries
- "Find HR Manager jobs in St. Petersburg FL"
- "Show me entry-level HR positions near Tampa Bay"
- "Any remote HR coordinator roles in Florida?"
- "What companies are hiring HR generalists in Pinellas County?"

## Project Structure
```
hr-job-search-agent/
├── index.html        # Main app (React + Anthropic API)
├── README.md         # This file
└── .env.example      # Environment variable template
```

## Deployment to GitHub Pages
1. Push to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your app will be live at `https://YOUR_USERNAME.github.io/hr-job-search-agent`

## Notes
- API calls are made directly from the browser to Anthropic's API
- Your API key is never stored persistently — only in the current session
- Web search is powered by Anthropic's built-in search tool

## License
MIT
