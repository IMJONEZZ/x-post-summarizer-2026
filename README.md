# X Post Summarizer 2026

AI-generated summary of a public figure's 2026 X posts, built with LangGraph, MCP tools, and the X API.

## Overview

This repository contains automated summaries of X/Twitter posts from notable figures in the AI/LLM community. The summaries are generated using:

- **LangGraph**: For orchestrating the summarization workflow
- **MCP Tools**: For GitHub repository management and file operations
- **X API**: For retrieving recent posts from target accounts

## Features

- Automated post retrieval from X/Twitter
- Structured markdown summaries with:
  - Overview
  - Key Themes
  - Notable Posts
  - Summary Statistics
- GitHub repository integration for storage and versioning

## Usage

The summarization process:
1. Fetches recent posts from a specified X/Twitter account
2. Analyzes content for themes and engagement patterns
3. Generates a structured markdown report
4. Saves the report to a GitHub repository

## Example Output

See `summaries/` directory for generated post summaries.

## Tech Stack

- Python
- LangGraph
- GitHub MCP Tools
- X/Twitter API v2

## License

MIT