# Code2Course Project Overview

## Stack
- **Backend:** Node.js
- **APIs:** GitHub API, OpenAI GPT-4
- **Database:** MongoDB
- **Frontend:** React

---

## Features & Flow

### 1. API Route: Analyze GitHub Repo
- **Input:** GitHub repo URL
- **Process:**
    - Fetch README and file structure via GitHub API
    - Identify key folders/files (e.g., `src/`, `components/`, `models/`)

### 2. GPT-4 Integration
- **Prompt:**  
    _"Turn the contents of this JavaScript/React project into a 5-part course. Include:  
    - Key concepts explained in simple terms  
    - Suggested reading links  
    - One quiz per concept  
    - Final project idea"_
- **Input:** Structure and code samples

### 3. Course JSON Structure
```json
{
    "title": "Lesson 1: React Components",
    "content": "...",
    "quiz": [
        {
            "question": "",
            "options": [],
            "answer": ""
        }
    ]
}
```

### 4. Storage
- Save generated course JSON in MongoDB under the user's profile

### 5. React Frontend
- Lesson & quiz navigation
- Progress tracking bar
- Dark/light mode toggle

---

## Monetization Model
- **Free:** 1 repo/month for personal use
- **Paid:** Educator plan with curriculum export features

---

## Next Steps
- [ ] Set up Node.js backend and connect to MongoDB
- [ ] Implement GitHub API integration
- [ ] Integrate OpenAI GPT-4 API
- [ ] Design React frontend components
- [ ] Add authentication and user profiles
- [ ] Implement monetization logic
