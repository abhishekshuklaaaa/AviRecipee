# AviRecipee

## Project Overview

**AviRecipee** is a web application designed to help users discover and search for recipes effortlessly. Leveraging the power of **[OpenSearch](https://opensearch.org/)**, it enables fast and accurate search results based on various filters like ingredients, dietary preferences, and more. The application provides a smooth, user-friendly interface built using **[React.js](https://reactjs.org/)** for the frontend, while **[Django](https://www.djangoproject.com/)** (Python) manages the backend. AviRecipee offers a modern solution for recipe searching and management, ensuring efficiency and an enjoyable user experience.

## Tech Stack

- **Frontend**: [React.js](https://reactjs.org/) – for building a dynamic and responsive user interface.
- **Backend**: [Django](https://www.djangoproject.com/) – for managing backend logic and API services.
- **Search Engine**: [OpenSearch](https://opensearch.org/) – for fast, scalable recipe searching and indexing.
- **Database**: SQLite / PostgreSQL (Specify which one you are using).
- **Version Control**: [Git](https://git-scm.com/) & [GitHub](https://github.com/) – for source code management and collaboration.

## Features

- **Recipe Search**: Users can search for recipes by title, ingredients, or dietary preferences.
- **Filtering**: Recipes can be filtered based on nutritional values such as protein, fat, and sodium.
- **User Authentication**: Basic user authentication for login and registration (Django).
- **Ratings & Reviews**: Users can rate and review recipes (optional).

## Prerequisites

Before you begin, ensure you have the following tools installed:

- [Python 3.x](https://www.python.org/downloads/)
- [Node.js](https://nodejs.org/en/download/)
- [OpenSearch](https://opensearch.org/)
- [Git](https://git-scm.com/)

## Installation

### Backend Setup (Django)

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/aviRecipee.git
   cd aviRecipee/backend
2. Create and activate a virtual environment:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate 
3. Install backend dependencies: 
    ```bash
    pip install -r requirements.txt
4. Run database migrations:
   ```bash
   python manage.py migrate
5. Start the Django development server:
   ```bash
   python manage.py runserver
### Frontend Setup (React) 
1. Navigate to the frontend directory: 
   ```bash
   cd ../frontend
2. Install dependencies:
   ```bash
   npm install
3. Start the React development server:
   ```bash
   npm start
## Usage

- Make sure **OpenSearch** is running at `http://localhost:9200`.
- Start both the **backend Django server** and the **frontend React app** as described in the installation steps.
- Open your browser and navigate to `http://localhost:3000` to access the AviRecipee application.

## API Endpoints

### Search Recipes
- **GET** `/api/recipes/search/`
- **Parameters**: `q`
- **Description**: This endpoint allows users to search for recipes by their title.

### Filter Recipes
- **GET** `/api/recipes/filter/`
- **Parameters**: `protein`, `fat`, `sodium`,`calories`,`rating`
- **Description**: This endpoint filters recipes based on nutritional values such as protein, fat, and sodium content.


Happy Cooking! 🍳✨
