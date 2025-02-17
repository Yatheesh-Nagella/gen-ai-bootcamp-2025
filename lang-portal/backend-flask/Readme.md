# README - Backend (Lang Portal)

## Overview

The backend of the **Lang Portal** project serves as a language learning inventory, a Learning Record Store (LRS), and a unified launchpad for study activities. This API-driven backend is built using **Flask** and **SQLite3** as the database.

## Features

- Stores vocabulary words, their meanings, and metadata.
- Tracks study sessions and review attempts.
- Provides paginated and sortable endpoints for words and groups.
- Supports study session creation and word review logging.
- No authentication required (assumes a single user scenario).

## Technology Stack

- **Language:** Python (Flask framework)
- **Database:** SQLite3
- **AI Coding Assistants Used:** Cursor, Windsurf Codeium, Github Copilot, Amazon Q Developer, Google Code Assist

## API Endpoints

### Words

- `GET /words` - Retrieve paginated list of words with review stats
  - Query Parameters: `page`, `sort_by`, `order`

### Groups

- `GET /groups` - Retrieve paginated list of word groups
  - Query Parameters: `page`, `sort_by`, `order`
- `GET /groups/:id` - Get words from a specific group

### Study Sessions

- `POST /study_sessions` - Create a new study session
  - Parameters: `group_id`, `study_activity_id`
- `POST /study_sessions/:id/review` - Log a word review attempt
  - Parameters: `word_id`, `correct`

## Database Schema

- **words** (Stores vocabulary)
- **groups** (Manages word collections)
- **word\_groups** (Many-to-many relationship between words and groups)
- **study\_activities** (Defines study types)
- **study\_sessions** (Tracks individual study sessions)
- **word\_review\_items** (Logs word reviews during sessions)

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the backend directory:
   ```bash
   cd lang-portal/backend-flask
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the application:
   ```bash
   python app.py
   ```

## Future Improvements

- Implement caching for frequent queries.
- Extend API with additional endpoints.
- Introduce optional authentication.