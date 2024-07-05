# Gemini Chatbot Interface with Streamlit

## Overview

This project is a Streamlit-based chat application that interacts with the Gemini AI model, allowing users to engage in conversations with an artificial intelligence assistant. The application stores chat history, allowing users to revisit and continue previous conversations.

## Getting Started

### Dependencies

This code uses the following libraries:

- `streamlit`: for building the user interface. 
- `gemini`: for chat  
- Gemini API key: Get it from [Google AI Studio](https://ai.google.dev/tutorials/setup?hl=tr)


### Usage

Follow these steps to set up and run the project:

1. Create a virtual environment:
```
python3 -m venv venv
source ./venv/bin/activate
```

2. Install dependencies:
```
pip install -r requirements.txt
```

3. Run the Streamlit server:
```
streamlit run app.py
```

4. Access the application in your browser at http://localhost:8501.

5. Start chatting with the assistant!

## Repository Structure
```
repository/
├── app.py               # the code and UI integrated together live here
├── requirements.txt     # the python packages needed to run locally
├── .streamlit/
│   └── config.toml      # theme info for the UI
├── data/                # folder for saved chat messages 
├── docs/                # preview for github

```

## How it Works

The app as follows:

1. The user enters a question in the input field.

2. User messages are sent to the Gemini model for processing.

3. The user's input, along with the chat history, is used to generate a response.

4. The Gemini model generates a response based on the patterns it learned during training.

5. The application saves chat messages and Gemini AI chat history to files for later retrieval.

6. A new chat is created if the user initiates a conversation that hasn't been stored before, or user can go back to past chats.
