# GitHub-Chat-App-with-LLaMA
## Overview

GitHub Chat App with LLaMA is a Streamlit-based application that allows users to interact with their GitHub repositories using a natural language model. The app loads repository details, processes user queries, and generates AI-powered responses using Meta's LLaMA model.

## Features

- Authenticate and connect to a GitHub account.
- Fetch and display repository details, including description, stars, forks, and files.
- Use an AI model to answer questions related to the repository.
- Supports GPU acceleration for efficient inference.

## Technologies Used

- **Streamlit** for the web-based UI.
- **Hugging Face Transformers** for AI-powered text generation.
- **PyGithub** for GitHub API integration.
- **Torch** for GPU-based model execution.

## Installation

Ensure you have Python installed, then install dependencies:

```bash
pip install streamlit torch transformers PyGithub
```

## Usage

1. **Run the application:**
   ```bash
   streamlit run gitchat.py
   ```
2. **Enter your GitHub credentials** in the UI.
3. **Select a repository** to fetch details.
4. **Ask questions** about the repository.
5. **Receive AI-generated responses** based on repository content.

## Environment Variables

The app requires a Hugging Face authentication token. Set it as an environment variable:

```bash
export HF_TOKEN='your_huggingface_token'
```

## How It Works

1. **Authentication**: Users enter GitHub credentials.
2. **Repository Fetching**: The app retrieves repo details using PyGithub.
3. **Model Loading**: The AI model is loaded with GPU support if available.
4. **User Queries**: Users ask questions about the repository.
5. **AI Response**: The model generates responses based on repo data.

## Future Enhancements

- Improved error handling for API calls.
- Multi-repository analysis support.
- Advanced AI models for better contextual understanding.
- Enhanced UI/UX for a smoother experience.


