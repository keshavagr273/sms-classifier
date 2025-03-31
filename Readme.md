# Email/SMS Spam Classifier

The Email/SMS Spam Classifier is a web application that allows users to classify messages as spam or not spam. The application uses a machine learning model to predict whether a given message is spam based on its content.

## Hosted Application

The application is hosted on Render. You can access it at [https://sms-classifier-ytit.onrender.com](https://sms-classifier-ytit.onrender.com).

## Features

- **Message Input**: Enter the message to be classified.
- **Text Preprocessing**: Convert text to lowercase, tokenize, remove stopwords and punctuation, and apply stemming.
- **Vectorization**: Transform the preprocessed text into a numerical format using TF-IDF vectorization.
- **Prediction**: Use a pre-trained machine learning model to predict if the message is spam or not.
- **Result Display**: Display the classification result as "Spam" or "Not Spam".

## Technologies Used

- **Python**: The programming language used for the application.
- **Streamlit**: The framework used to create the web application.
- **NLTK**: The Natural Language Toolkit used for text preprocessing.
- **scikit-learn**: The machine learning library used for model training and prediction.
- **Pickle**: Used for loading the pre-trained model and vectorizer.
- **PyCharm**: The IDE used for development.

## Installation

1. Clone the repository:
    ```bash
    git clone <repository-url>
    ```
2. Navigate to the project directory:
    ```bash
    cd <project-directory>
    ```
3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```
4. Download the necessary NLTK data:
    ```bash
    python -m nltk.downloader -d /usr/local/share/nltk_data -u nltk.txt
    ```

## Usage

1. Run the Streamlit application:
    ```bash
    streamlit run app.py
    ```
2. Open the web browser and go to the provided URL.
3. Enter the message in the text area and click the "Predict" button to classify the message.

## Files

- `app.py`: The main application file containing the Streamlit code and the text preprocessing function.
- `requirements.txt`: The file listing the required Python packages.
- `nltk.txt`: The file listing the NLTK data to be downloaded.
- `vectorizer.pkl`: The pre-trained TF-IDF vectorizer.
- `model.pkl`: The pre-trained machine learning model.

## Acknowledgements

A special thanks to Nitish Singh for his elaborate and simple explanation.