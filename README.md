# Personalized Recipe Recommender (2024)

This is a personalized recipe recommendation system that uses Flask, MongoDB, and React. It suggests recipes based on user preferences and dietary restrictions. The app scrapes real-time recipe data, stores it in MongoDB, and provides recommendations using a basic machine learning algorithm.

## Tech Stack:
- **Backend:** Flask, Python, MongoDB
- **Frontend:** React, JavaScript, Axios
- **Scraping:** BeautifulSoup (Python)
- **Recommendation Logic:** Basic filtering based on user preferences (e.g., vegetarian, vegan)

## Project Folder Structure:
personalized-recipe-recommender/ │ ├── backend/ │ ├── app.py │ ├── requirements.txt │ ├── models.py │ ├── recipe_scraper.py │ └── recommendation_engine.py │ └── frontend/ ├── public/ │ └── index.html ├── src/ │ ├── App.js │ ├── components/ │ │ └── RecipeList.js │ ├── styles/ │ │ └── App.css │ └── index.js └── package.json



## Features:
- **Scraping:** The backend scrapes recipe data from an online source and stores it in a MongoDB database.
- **Personalized Recommendations:** The system filters recipes based on dietary preferences (e.g., vegetarian, vegan, gluten-free).
- **Real-Time Data:** The app pulls real-time recipe data from multiple online sources and presents up-to-date recommendations.

## How to Run the Project:

### 1. Setup the Backend (Flask):
- **Step 1:** Create a virtual environment for the Python backend:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use: 'venv\Scripts\activate'
    ```

- **Step 2:** Install the required dependencies:
    ```bash
    pip install -r backend/requirements.txt
    ```

- **Step 3:** Run the Flask app:
    ```bash
    python backend/app.py
    ```

This will start the Flask API server on `http://localhost:5000`.

### 2. Setup the Frontend (React):
- **Step 1:** Navigate to the frontend folder and install the necessary dependencies:
    ```bash
    cd frontend
    npm install
    ```

- **Step 2:** Start the React app:
    ```bash
    npm start
    ```

This will start the React app on `http://localhost:3000`.

### 3. Usage:
- Open your browser and go to `http://localhost:3000` to use the app.
- You can select your dietary preferences from a dropdown menu (e.g., Vegetarian, Vegan, Gluten-Free).
- Click "Get Recipe Recommendations" to see a list of recipes based on your preferences.
- Recipes are linked to their original sources.

### 4. API Endpoints:
- **POST `/api/recommend`**: This endpoint receives a JSON object containing user preferences (e.g., `{"dietary": "vegetarian"}`) and returns a list of recommended recipes.
- **GET `/api/scrape`**: This endpoint scrapes recipe data from an online source and stores it in the MongoDB database. This can be triggered manually as needed.

## License:
MIT License





