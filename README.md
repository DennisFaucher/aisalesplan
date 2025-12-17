# Perplexity Docker Web Application

A Dockerized web application for searching customer AI research using the Perplexity API.

## Features

- Web-based interface with "Customer AI Sales Plan" form
- Enter customer name and click "Go" to search
- Results displayed as HTML table with footnotes and URLs
- Export results to an editable Microsoft Word document (.docx)
- Dockerized for easy deployment

## Prerequisites

- Docker
- Docker Compose

## Setup

1. Set your Perplexity API key (optional, defaults to the one in docker-compose.yml):
   ```bash
   export PERPLEXITY_API_KEY='your_api_key_here'
   ```

2. Build and run with Docker Compose:
   ```bash
   docker compose up --build
   ```

3. Open your browser and navigate to:
   ```
   http://localhost:5000
   ```

## Usage

1. Enter a customer name in the input field
2. Click the "Go" button
3. Wait for the search to complete
4. View the results in the HTML table below

## Stopping the Application

Press `Ctrl+C` in the terminal, or run:
```bash
docker compose down
```

## Environment Variables

- `PERPLEXITY_API_KEY`: Your Perplexity API key (optional, can be set in docker-compose.yml)

