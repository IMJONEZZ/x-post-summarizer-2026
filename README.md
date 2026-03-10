# X Post Summarizer 2026

AI-generated summary of a public figure's 2026 X posts, built with LangGraph, MCP tools, and the X API.

## Overview

This repository contains automated summaries of X/Twitter posts from notable figures in the AI/LLM community. The summaries are generated using:

- **LangGraph**: For orchestrating the summarization workflow
- **MCP Tools**: For GitHub repository management and file operations
- **X API**: For retrieving recent posts from target accounts

## Project Description

This project summarizes a public figure's 2026 X posts using AI-powered analysis. The system:

1. **Retrieves posts** from a specified X/Twitter account using the X API v2
2. **Analyzes content** for themes, engagement patterns, and notable posts
3. **Generates structured markdown summaries** with overview, key themes, notable posts, and statistics
4. **Stores results** in a GitHub repository with version control

### Account Analyzed

- **Handle:** @llm_wizard
- **Date Range:** March 6–9, 2026
- **Posts Analyzed:** 20

## How It Was Built

This project was built using a **LangGraph agent** that orchestrates the following workflow:

1. **X API v2 Integration**: Retrieves recent posts from the target account
2. **Content Analysis**: Identifies themes, engagement metrics, and notable posts
3. **GitHub MCP Tools**: Manages repository operations including:
   - Creating repositories
   - Committing files (README, summaries, metadata)
   - Creating branches and pull requests
   - Managing file versions

## Replicating This Process

### Prerequisites

- Python 3.8+
- X/Twitter API v2 Bearer Token
- GitHub account with API access

### Step 1: Set Up X API Bearer Token

1. Go to [Twitter Developer Portal](https://developer.twitter.com/)
2. Create a new project and app
3. Generate a Bearer Token
4. Set it as an environment variable:

```bash
export X_BEARER_TOKEN="your_bearer_token_here"
```

### Step 2: Install Python Dependencies

```bash
pip install requests python-dotenv
```

### Step 3: Run the Search Script

```bash
# Search for posts from a specific user
python x_search.py <username>

# Example:
python x_search.py llm_wizard
```

This will:
- Fetch recent posts from the specified account
- Save results to `posts.json`
- Display a summary of found posts

### Step 4: Generate Summary

Use a LangGraph agent or similar AI workflow to:
1. Load the posts from `posts.json`
2. Analyze content for themes and patterns
3. Generate a structured markdown summary
4. Save to `summary.md`

### Step 5: Create GitHub Repository

Use GitHub MCP tools or the GitHub API to:
1. Create a new repository
2. Commit the README, summary, and metadata files
3. Create branches for additional features
4. Open pull requests for review

## Files in This Repository

| File | Description |
|------|-------------|
| `README.md` | Project documentation |
| `summary.md` | Generated X post summary for @llm_wizard |
| `metadata.json` | Analysis metadata (on `add-metadata` branch) |
| `x_search.py` | X API search script |

## Tech Stack

- Python
- LangGraph
- GitHub MCP Tools
- X/Twitter API v2
- requests

## License

MIT