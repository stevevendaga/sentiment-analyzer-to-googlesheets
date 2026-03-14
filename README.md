# Sentiment Analysis to Google Sheets Workflow

A workflow that captures user reviews through a web form, analyzes their sentiment using AI, and automatically stores the data in Google Sheets.

## Features

- **Web Form**: Collects user input including name and review text
- **AI-Powered Sentiment Analysis**: Uses OpenAI's GPT model to classify reviews as Positive, Negative, or Neutral
- **Automated Data Storage**: Appends collected data directly to Google Sheets
- **Real-time Processing**: Processes each form submission instantly

## How It Works

1. User submits a form with their name and review
2. System extracts the review text and sends it to the AI model
3. AI determines the sentiment (Positive/Negative/Neutral) from the review
4. All data (name, review, and sentiment) is combined and saved to Google Sheets

## Setup Requirements

- OpenAI API key for sentiment analysis
- Google Sheets API credentials
- Access to create webhooks for form submissions

## Data Flow

- **Form Trigger** → Captures user input
- **LLM Chain** → Processes review text with AI
- **Merge Node** → Combines all data points
- **Google Sheets Node** → Stores complete records in spreadsheet

## Use Cases

- Customer feedback collection and analysis
- Social media monitoring
- Product review tracking
- Survey response processing