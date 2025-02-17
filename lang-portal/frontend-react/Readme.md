# README - Frontend (Lang Portal)

## Overview

The frontend of **Lang Portal** is a web-based interface for a language learning prototype. It provides an interactive UI to browse vocabulary, track study sessions, and launch study activities. The application is powered by the backend API.

## Features

- Displays vocabulary with filtering and sorting options.
- Provides access to word groups and study sessions.
- Offers a responsive UI for an enhanced learning experience.
- Uses AI prototyping services for faster development.

## Technology Stack

- **Language:** TypeScript
- **CSS Framework:** Tailwind CSS
- **Build Tool:** Vite.js
- **UI Components:** ShadCN
- **AI Prototyping Services:** Lovable.dev, Bolt.new, v0.dev
- **AI Coding Assistants:** Cursor, Windsurf Codeium, Github Copilot, Amazon Q Developer, Google Code Assist

## Folder Structure

```
frontend-react/
├── public/               # Static assets
├── src/
│   ├── components/       # UI Components
│   ├── context/          # Context Providers
│   ├── hooks/            # Custom Hooks
│   ├── pages/            # Page Components
│   ├── services/         # API Calls
│   ├── lib/              # Utility Functions
│   ├── assets/           # Images and icons
│   ├── App.tsx           # Main Application Component
│   ├── main.tsx          # Entry Point
├── package.json          # Project Dependencies
├── tailwind.config.js    # Tailwind CSS Configuration
├── vite.config.ts        # Vite Configuration
```

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the frontend directory:
   ```bash
   cd lang-portal/frontend-react
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Start the development server:
   ```bash
   npm run dev
   ```

## Future Improvements

- Add more interactive study activities.
- Implement performance optimizations.
- Enhance UI with additional animations and themes.