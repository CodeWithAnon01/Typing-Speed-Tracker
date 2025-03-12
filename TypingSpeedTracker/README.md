# Typing Speed Test Game (C++ Backend with Crow)

## Project Overview
This project is a **Typing Speed Test Tracker** that evaluates a user's typing speed in **words per minute (WPM)** and **characters per minute (CPM)** while tracking mistakes. The frontend is built using **HTML and CSS**, while the backend is implemented in **C++ using the Crow web framework** to handle logic and user interactions using **Object-Oriented Programming (OOP)** principles.

## Features
- Displays a randomly selected paragraph for typing.
- Tracks WPM, CPM, mistakes, and remaining time.
- Backend handles game logic and updates data dynamically.
- Uses OOP concepts such as **classes, encapsulation, inheritance, and polymorphism**.
- Implements **RESTful APIs** using Crow to interact with the frontend.

## Technologies Used
### Frontend:
- **HTML** (Structure)
- **CSS** (Styling)

### Backend:
- **C++** (Core logic)
- **Crow Library** (Web framework for API handling)

## Project Structure
```
TypingTestGame/
│── frontend/
│   ├── index.html        # Main UI structure
│   ├── style.css         # Styling for the UI
│── backend/
│   ├── main.cpp          # Main entry point (Crow server)
│   ├── GameManager.h     # Header file for game logic
│   ├── GameManager.cpp   # Implementation of game logic
│── assets/
│   ├── paragraphs.txt    # List of predefined paragraphs
│── README.md             # Project Documentation
```

## Installation and Setup
### Prerequisites
- C++ Compiler (e.g., g++)
- Crow library
- Basic web browser (for frontend testing)

### Steps to Run the Project
1. **Clone the Repository:**
   ```sh
   git clone <repo_link>
   cd TypingTestGame
   ```
2. **Install Crow Library:**
   ```sh
   # If using vcpkg
   vcpkg install crow
   ```
3. **Compile and Run the Backend:**
   ```sh
   g++ backend/main.cpp backend/GameManager.cpp -o server -I/usr/include -L/usr/lib -lcrow -std=c++17
   ./server
   ```
4. **Open the Frontend in Browser:**
   - Open `frontend/index.html` in any web browser.

## API Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/getParagraph` | Fetches a random paragraph |
| POST | `/submitTyping` | Receives typing data and calculates WPM, CPM, and mistakes |
| GET | `/resetGame` | Resets the game state |

## Object-Oriented Concepts Used
- **Encapsulation**: The `GameManager` class encapsulates game logic.
- **Inheritance**: The `TypingTest` class extends core game functionality.
- **Polymorphism**: Different typing modes can be handled through method overriding.
- **Abstraction**: The game logic is hidden from the frontend and accessed via APIs.

## Future Enhancements
- Add difficulty levels (easy, medium, hard).
- Store high scores in a local file.
- Implement a leaderboard system.

## Contributors
- **Minhal Raza** *(Project Lead & UI/Frontend Developer)*
- **Ali Rooman** *(OOP Logic Developer)*
- **Madni Moazzam** *(Server-Side & API Developer)*

## License
This project is **open-source**.

