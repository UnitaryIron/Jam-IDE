# Jam IDE

A simple **web-based IDE** for the Jam programming language.  
The IDE is built using **HTML, CSS, and JavaScript** (with the Monaco editor) and connects to a **Flask backend** for running Jam code.

---

## Table of Contents
- [Features](#features)
- [Setup](#setup)
  - [1. Clone this repo](#1-clone-this-repo)
  - [2. Install backend dependencies](#2-install-backend-dependencies)
  - [3. Run the backend](#3-run-the-backend)
  - [4. Open the IDE](#4-open-the-ide)
- [Usage](#usage)
- [Deployment](#deployment)
- [Tech Stack](#tech-stack)
- [Contributing](#contributing)
- [License](#license)

---

## Features
- Monaco editor with Jam syntax highlighting & autocomplete
- Run Jam code directly from the browser
- Compile Jam code to JavaScript
- Dark-themed interface
- Lightweight, runs entirely in the browser + a simple Flask API

---

## Setup

### 1. Clone this repo
```bash
git clone https://github.com/yourusername/jam-ide.git
cd jam-ide
```

### 2. Install backend dependencies
```bash
pip install flask flask-cors
```

### 3. Run the backend
```bash
cd backend
python app.py
```
The backend will start at:
```bash
http://localhost:5000/run
```

### 4. Open the IDE
Simply open index.html in your browser.

## Usage

- Write Jam code in the editor.
- Click Run to send it to the backend and see output.
- Click Compile to JS to view the JavaScript translation.
- Click Clear Output to reset the console.

## Deployment

The backend can be deployed on Render, Railway, or Heroku.
Update the fetch() URL in index.html to point to your deployed backend:

```js
const res = await fetch("https://your-backend.onrender.com/run", { ... });
```

## Tech Stack

- Frontend: HTML, CSS, JavaScript, Monaco Editor
- Backend: Python, Flask, Flask-CORS

## Contributing
Pull requests and issues are welcome!
If you’d like to add features (like Jam file management, error highlighting, or REPL mode), feel free to open a PR.

## License
MIT License — free to use, modify, and distribute.
