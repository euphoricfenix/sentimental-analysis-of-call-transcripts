
# Sentiment Analysis on Call Transcripts

This project provides a web application for performing sentiment analysis on call transcripts using a pre-trained DistilBERT model. The application allows users to upload text files and receive sentiment analysis results in real-time.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Features

- Upload call transcripts in TXT format.
- Perform sentiment analysis using a pre-trained DistilBERT model.
- View sentiment analysis results in a user-friendly interface.
- Log errors and processing information for debugging.

## Technologies Used

- Python
- Flask (for the backend)
- Streamlit (for the frontend)
- Transformers (Hugging Face library for NLP)
- PyTorch (for model inference)
- CORS (for cross-origin requests)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/sentiment-analysis-call-transcripts.git
   cd sentiment-analysis-call-transcripts
   ```

2. Create a virtual environment (optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

   Make sure to include the following in your `requirements.txt`:

   ```
   Flask
   Flask-CORS
   transformers
   torch
   streamlit
   ```

## Usage

1. Start the backend server:

   ```bash
   python backend.py
   ```

2. In a new terminal, start the frontend application:

   ```bash
   streamlit run frontend.py
   ```

3. Open your web browser and navigate to `http://localhost:8501` to access the application.

4. Upload a call transcript in TXT format and view the sentiment analysis results.

## API Endpoints

### Upload Endpoint

- **URL**: `/upload`
- **Method**: `POST`
- **Description**: Upload a text file for sentiment analysis.
- **Request**: 
  - Form-data with key `file` containing the text file.
- **Response**: 
  - JSON object with sentiment analysis results or error messages.

### Test Endpoint

- **URL**: `/test`
- **Method**: `GET`
- **Description**: Check if the server is running.
- **Response**: 
  - JSON object with status message.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for any suggestions or improvements.

