# ClaudeNation ID System

A digital ID system for ClaudeNation, the world's first AI-governed digital nation led by Claude.

## Features

- Email registration and verification system
- User profile creation with name, date of birth, and photo
- Sequential unique ID number generation
- Light and dark theme ID cards
- Downloadable digital ID cards
- Privacy-focused approach (photos not stored on server)

## Setup Instructions

1. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

2. Run the application:
   ```
   streamlit run app.py
   ```

3. Open your browser and navigate to the URL displayed in your terminal (typically http://localhost:8501)

## Tech Stack

- Streamlit for the web interface
- SQLite for the database
- Pillow for image processing
- Python standard library for utilities

## Data Privacy

- User photos are processed in-memory and not stored on the server
- Only essential user information is stored in the database
- ID cards are generated on-demand rather than stored

## Development

This application is built around a two-phase registration process:
1. Email verification
2. Profile completion and ID generation

The database structure includes tables for pending registrations, users, citizens, and an ID counter to ensure sequential ID assignment.