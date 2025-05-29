# 🌍 Global News Portal

A sleek and fast news application that delivers news articles from around the world with a focus on speed, visualization, and usability. This project uses a third-party API from [NewsAPI](https://newsapi.org/) to fetch real-time news data.

## 🚀 Features

- 🌐 Aggregates news articles from trusted sources globally
- ⚡ Fast and efficient performance
- 🎨 Clean and responsive UI for optimal readability
- 📊 Categorized news display (e.g., politics, sports, entertainment, finance, etc.)
- 🔄 Real-time updates using [NewsAPI](https://newsapi.org/)

## 🖥️ Tech Stack

- HTML, CSS, JavaScript
- NewsAPI (for fetching live news articles)
- [Live Server Extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) (for local development)

---

## API Fallback (Optional)
- If you don’t want to use the live API during development or your API key is not working, you can use a local JSON file (news.json) that   contains sample news data.

In script.js, comment/uncomment the relevant lines as needed:

async function fetchNews(query) {
    // ✅ Live API (default)
    const res = await fetch(`${url}${query}&apiKey=${API_KEY}`);

    // 🧪 Uncomment the line below to use local dummy data instead
    // const res = await fetch("news.json"); 

    const data = await res.json();
    bindData(data.articles);
}

## 🔧 Getting Started

### 📁 Clone the Repository

```bash
git clone https://github.com/jyraut/News-Application.git
cd News-Application
