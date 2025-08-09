# AI-Powered Fake News Detector

[![React](https://img.shields.io/badge/Frontend-React-blue.svg)](https://reactjs.org/)
[![Django](https://img.shields.io/badge/Backend-Django-darkgreen.svg)](https://www.djangoproject.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A web application designed to detect fake news articles using machine learning. The goal of this project is to provide a tool that can help users identify unreliable news sources and combat the spread of misinformation.

## Table of Contents
- [Overview](#overview)
- [Key Features](#key-features)
- [Technology Stack](#technology-stack)
- [Getting Started](#getting-started)
- [Contributing](#contributing)
- [Future Enhancements](#future-enhancements)
- [License](#license)

## Overview
FND is a web-based application that uses machine learning models to analyze news articles and predict whether they are real or fake. This project was initially developed as part of college coursework and has been refined to serve as a practical tool in the fight against digital misinformation.

## Key Features
- **Live News Monitoring:** View real-time predictions for news articles as they are analyzed by the model.
- **News Quiz:** Test your own ability to detect fake news by taking an interactive quiz.
- **Check by Title:** Quickly check a news article's authenticity by entering its title.
- **User Collaboration:** The project is open for collaboration to encourage further improvements and feature development.

## Technology Stack
- **Backend:** Python, Django, Django REST Framework
- **Frontend:** React, JavaScript (ES6+)
- **AI / Machine Learning:** Scikit-learn, NLTK, Pandas
- **Database:** SQLite (for development)

## Getting Started
To get this project running on your local machine, follow the setup instructions for both the backend and frontend.

### Backend Setup (Django API)

1.  **Navigate to the backend directory:**
    ```sh
    cd app/FakeNewsDetectorAPI/
    ```
2.  **Create and activate a virtual environment (Recommended):**
    ```sh
    # For Windows
    python -m venv venv
    venv\Scripts\activate

    # For macOS/Linux
    python3 -m venv venv
    source venv/bin/activate
    ```
3.  **Install Python dependencies:**
    ```sh
    pip install -r requirements.txt
    ```
4.  **Run database migrations:**
    ```sh
    python manage.py migrate
    ```
5.  **Run the development server:**
    ```sh
    python manage.py runserver
    ```
    The backend API will now be running at `http://127.0.0.1:8000/`.

6.  **(Optional) Load quiz data:**
    To populate the news quiz, run this command from the `app/FakeNewsDetectorAPI/` directory.
    ```sh
    python manage.py quiz_data_loader path/to/your/game_data.csv
    ```

### Frontend Setup (React App)

1.  **Open a new terminal** and navigate to the frontend directory:
    ```sh
    cd app/fake-news-detector-frontend/
    ```
2.  **Install JavaScript dependencies:**
    ```sh
    npm install
    ```
3.  **Run the development server:**
    ```sh
    npm start
    ```
    The React application will open automatically in your browser at `http://localhost:3000`.

## Contributing
Contributions from fellow developers are welcome! If you have ideas for new features, improvements, or bug fixes, please feel free to open an issue or submit a pull request.

## Future Enhancements
- **Enhanced ML Models:** Improve the accuracy and performance of the fake news detection models.
- **User Profiles:** Allow users to create profiles to track quiz scores and history.

## License
This project is distributed under the MIT License. See the `LICENSE` file for more information.
