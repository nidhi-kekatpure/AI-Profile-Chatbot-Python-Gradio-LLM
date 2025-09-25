# Nidhi Kekatpure - AI Personal Chatbot

AI-powered personal chatbot that represents Nidhi Kekatpure's professional profile using OpenAI GPT and Gradio interface.

## Overview

This project creates an interactive chatbot that can answer questions about Nidhi Kekatpure's career, background, skills, and experience. The chatbot uses OpenAI's GPT model to provide professional and engaging responses based on her LinkedIn profile and personal summary.

## Features

- **AI-Powered Conversations**: Uses OpenAI GPT-4o-mini for intelligent responses
- **Professional Context**: Trained on LinkedIn profile data and personal summary
- **Web Interface**: Interactive chat interface built with Gradio
- **PDF Processing**: Extracts information from LinkedIn PDF profile
- **Response Evaluation**: Built-in evaluation system using Google's Gemini model

## Technologies Used

- **Python**: Core programming language
- **OpenAI GPT-4o-mini**: Main conversational AI model
- **Google Gemini 2.0 Flash**: Response evaluation model
- **Gradio**: Web interface for the chatbot
- **PyPDF2**: PDF text extraction
- **Pydantic**: Data validation and parsing
- **python-dotenv**: Environment variable management

## Project Structure

```
├── Chatbot_NidhiProfile.ipynb    # Main Jupyter notebook with implementation
├── profile/
│   ├── summary.txt               # Personal summary text
│   └── linkedin.pdf             # LinkedIn profile PDF (not in repo)
├── .env                         # Environment variables (not in repo)
├── .gitignore                   # Git ignore file
└── README.md                    # This file
```

## Setup Instructions

### Prerequisites

- Python 3.7+
- OpenAI API key
- Google API key (for evaluation features)

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd <repository-name>
```

2. Install required packages:
```bash
pip install openai gradio PyPDF2 python-dotenv pydantic
```

3. Create a `.env` file in the root directory:
```env
OPENAI_API_KEY=your_openai_api_key_here
GOOGLE_API_KEY=your_google_api_key_here
```

4. Add your LinkedIn profile PDF to the `profile/` directory as `linkedin.pdf`

### Running the Application

1. Open the Jupyter notebook:
```bash
jupyter notebook Chatbot_NidhiProfile.ipynb
```

2. Run all cells in the notebook

3. The Gradio interface will launch locally at `http://127.0.0.1:7861`

## Usage

Once the application is running:

1. Open the provided local URL in your browser
2. Start chatting with the AI representation of Nidhi Kekatpure
3. Ask questions about her:
   - Professional experience
   - Technical skills
   - Educational background
   - Career achievements
   - Project experience

## Key Components

### System Prompt
The chatbot is configured with a comprehensive system prompt that:
- Establishes the AI's role as Nidhi Kekatpure
- Provides context from LinkedIn profile and summary
- Sets professional and engaging tone guidelines
- Ensures accurate representation of her background

### Evaluation System
Includes an automated evaluation system that:
- Assesses response quality and appropriateness
- Uses Google's Gemini model for evaluation
- Provides structured feedback on chatbot responses
- Ensures professional standards are maintained

## Data Sources

- **Personal Summary**: Brief background information in `profile/summary.txt`
- **LinkedIn Profile**: Comprehensive professional information extracted from PDF
- **Contact Information**: Professional contact details and social links

## Security Notes

- API keys are stored in environment variables
- LinkedIn PDF and environment files are excluded from version control
- No sensitive personal information is hardcoded in the repository

## Contributing

This is a personal portfolio project. If you'd like to create a similar chatbot for yourself:

1. Fork the repository
2. Replace the profile data with your own information
3. Update the system prompt with your details
4. Customize the evaluation criteria as needed

---

*This chatbot represents Nidhi Kekatpure's professional profile and is designed to provide accurate information about her career, skills, and experience in an engaging conversational format.*
