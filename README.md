# Personalized Recipe Recommender (2024)

This is a personalized recipe recommendation system that uses Flask, MongoDB, and React. It suggests recipes based on user preferences and dietary restrictions. The app scrapes real-time recipe data, stores it in MongoDB, and provides recommendations using a basic machine learning algorithm.

## Tech Stack:
- **Backend:** Flask, Python, MongoDB
- **Frontend:** React, JavaScript, Axios
- **Scraping:** BeautifulSoup (Python)
- **Recommendation Logic:** Basic filtering based on user preferences (e.g., vegetarian, vegan)

## Project Folder Structure:
personalized-recipe-recommender/ │ ├── backend/ │ ├── app.py │ ├── requirements.txt │ ├── models.py │ ├── recipe_scraper.py │ └── recommendation_engine.py │ └── frontend/ ├── public/ │ └── index.html ├── src/ │ ├── App.js │ ├── components/ │ │ └── RecipeList.js │ ├── styles/ │ │ └── App.css │ └── index.js └── package.json



