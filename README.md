# Recipe Recommender AI

## Overview

Recipe Recommender AI is a multi-agent application that provides personalized recipe recommendations based on user dietary restrictions, preferences, and available ingredients. The system uses a team of AI agents that collaborate to fetch, filter, and recommend recipes tailored to individual user needs.

## Features

- Collect user dietary restrictions, preferences, and available ingredients.
- Fetch recipes from various online sources.
- Filter recipes based on user-specific criteria.
- Recommend personalized recipes.
- Deliver recommended recipes to the user via email.

## Technologies Used

- **LangGraph Framework**: To build and design the workflow of the AI agents.
- **Tavily API**: For enhanced filtering capabilities and Retrieval-Augmented Generation (RAG).
- **Spoonacular API**: To fetch recipes from an extensive database.
- **Flask**: For handling backend operations.
- **HTML/CSS/JavaScript**: For the frontend interface.
- **python-dotenv**: To manage environment variables securely.

## Installation

### Prerequisites

- Python 3.6 or higher
- pip
- Git

### Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/christopherthai/recipe-recommender-ai.git
   cd recipe-recommender-ai
   ```

2. **Create and Activate a Virtual Environment**

   ```bash
   python -m venv venv
   source venv/bin/activate
   # On Windows, use `venv\Scripts\activate`
   ```

3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up Environment Variables**

   - Create a `.env` file in the root directory of the project.
   - Add your API keys in the `.env` file:

   ```plaintext
   TAVILY_API_KEY=your_tavily_api_key_here
   SPOONACULAR_API_KEY=your_spoonacular_api_key_here
   ```

5. **Run the Application**

   ```bash
   python app.py
   ```

## Usage

1. Open your web browser and navigate to `http://127.0.0.1:5000/`.
2. Fill out the form with your dietary restrictions, preferences, and available ingredients.
3. Submit the form to receive personalized recipe recommendations.

## Project Structure

- `app.py`: Main Flask application file.
- `tavily_helper.py`: Helper functions to interact with the Tavily API.
- `recipe_database_agent.py`: Functions to fetch recipes from the Spoonacular API.
- `templates/index.html`: HTML file for the user input form.
- `static/script.js`: JavaScript file to handle form submission.
- `.env`: Environment variables file (not included in the repository).

## Contribution

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

If you have any questions or suggestions, feel free to contact me at [christopherthai.nyli@gmail.com](mailto:christopherthai.nyli@gmail.com).
