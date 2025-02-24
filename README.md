# DAL-News 📰

Welcome to **DAL-News**, an innovative news aggregation platform that brings the latest stories from diverse RSS feeds to your fingertips! Powered by Flask, Elasticsearch, and a sleek frontend, DAL-News lets you explore articles by category, search with fuzzy matching, and dive into detailed article pages with related content. Whether you're a news junkie or a developer looking to tinker, this project has something for you.

Deployed on [Render](https://render.com/), DAL-News is ready to scale, but you can also run it locally or deploy it elsewhere. Let’s get started!

## Features ✨

- **Dynamic Categories**: Browse news from "Top", "Sports", "World", "States", "Cities", "Entertainment", and custom filters like Karnataka and Bengaluru.
- **Smart Search**: Fuzzy search across titles and content for quick article discovery.
- **Article Details**: View summaries, images, and publication dates, with related articles powered by Elasticsearch’s `more_like_this`.
- **Multilingual Support**: Translate articles into languages like Spanish or French on the fly.
- **Real-Time Updates**: Fetch fresh RSS content with a simple API call.
- **Analytics**: Track usage with [Google Analytics](https://analytics.google.com/analytics/web/#/report-home/G-Y98XYMVPD8) (ID: `G-Y98XYMVPD8`).

## Tech Stack 🛠️

- **Backend**: Flask (Python), Elasticsearch Cloud
- **Frontend**: HTML, CSS, JavaScript (with dynamic rendering)
- **Data**: RSS feeds (NDTV), parsed with `feedparser`
- **Deployment**: Render (with alternatives like Heroku or Docker)

## Prerequisites 📋

To build, run, or deploy DAL-News, you’ll need:
- [Python 3.8+](https://www.python.org/downloads/) - The backbone of the app.
- [Git](https://git-scm.com/downloads) - For version control and cloning.
- [Elasticsearch Cloud](https://www.elastic.co/cloud) - Sign up for a free trial or paid plan.
- A code editor (e.g., [VS Code](https://code.visualstudio.com/), [PyCharm](https://www.jetbrains.com/pycharm/)).
- Optional: [Docker](https://www.docker.com/get-started) for containerized deployment.

## Project Structure 🌳

```plaintext
DAL-News/
  ├── static/              # Frontend assets
  │   ├── styles.css       # Custom styles
  │   ├── script.js        # Dynamic JavaScript
  │   └── news_logo.jpg    # Logo image
  ├── templates/           # HTML templates
  │   ├── index.html       # Homepage
  │   └── article.html     # Article details
  ├── app.py               # Core Flask app
  ├── DataExtractor.py     # RSS scraping and indexing
  ├── Translator.py        # Language translation
  ├── category.py          # Category filtering
  ├── search.py            # Search logic
  ├── requirements.txt     # Python dependencies
  ├── Dockerfile           # Optional Docker setup
  └── README.md            # You’re here!
