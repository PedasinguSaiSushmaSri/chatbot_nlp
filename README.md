# chatbot_nlp

# Chatbot Project

This project implements a chatbot using Flask with a web interface for user interaction. The chatbot processes questions and provides answers based on a preprocessed dataset.

## Features

- **User-Friendly Interface**: A simple web interface built with HTML, CSS, and Flask.
- **Preprocessed Dataset**: Uses tokenization, stopword removal, and lemmatization for efficient question matching.
- **Fuzzy Matching**: Handles similar questions using fuzzy matching.

## Installation

1. Clone this repository:
    ```
    git clone https://github.com/your-username/chatbot-project.git
    cd chatbot-project
    ```

2. Install dependencies:
    ```
    pip install -r requirements.txt
    ```

3. Download necessary NLTK data:
    ```
    python -m nltk.downloader punkt stopwords wordnet averaged_perceptron_tagger
    ```

4. Run the data preparation script:
    ```
    python data_preparation.py
    ```

5. Run the application:
    ```
    python app.py
    ```

6. Open a browser and navigate to `http://127.0.0.1:5000/`.

## Project Structure

project/
|---- app.py # Main Flask application file
|---- data_preparation.py # Script for preprocessing dataset
|---- templates/
| |---- index.html # HTML template for web interface
|---- static/
| |---- style.css # CSS file for styling the interface
|---- requirements.txt # List of dependencies for the project
|---- README.md # Project documentation file
|---- questions_answers.csv # Original dataset of questions and answers
|---- processed_questions_answers.csv # Preprocessed dataset for chatbot use
