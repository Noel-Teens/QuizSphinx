# 🧠 QuizSphinx – Unity Quiz Game

QuizSphinx is a cleanly architected **Unity-based multiple-choice quiz game** designed to demonstrate best practices in **game logic separation, ScriptableObject-driven data management, UI handling, and time-based gameplay mechanics**.

This project prioritizes **readability, scalability, and learning**, making it suitable for beginners, intermediate Unity developers, and portfolio showcasing.

---

## 🎮 Game Overview

QuizSphinx challenges players with a sequence of multiple-choice questions under a time limit.  
Each question requires quick decision-making and provides immediate visual feedback.

### Core Gameplay Loop
1. Display a question with four answer options
2. Player has **30 seconds** to select an answer
3. Correct answer is revealed for **10 seconds**
4. Game proceeds to the next question
5. Final score is shown as a percentage

The game is intentionally simple in UI but structured using **production-ready architectural patterns**.

---

## ✨ Features

- ⏱️ Dual-phase timer (answer + reveal)
- 📦 ScriptableObject-based question system
- 🎯 Real-time score tracking
- 📊 Percentage-based final result
- 🎨 Visual feedback for correct & incorrect answers
- 🧩 Reusable UI prefabs
- 🧠 Clean separation of data, logic, and UI
- 🔁 Replayable game session

---

## 🏗️ Architecture Overview

QuizSphinx follows a **modular and loosely coupled architecture**:

```

GameManager
├── Quiz (UI + Question Handling)
├── Timer (Time Control)
├── ScoreKeeper (Global Score State)
└── EndScreen (Final Result UI)

```

### Architectural Principles Used
- Single Responsibility Principle
- Data-driven design using ScriptableObjects
- Minimal scene dependencies
- Inspector-driven configuration
- Reusable and extendable components

---

## 🧠 Core Systems Explained

### 📝 Question System (ScriptableObjects)

Questions are stored as ScriptableObjects instead of hardcoded values.

Each question contains:
- Question text
- Four answer options
- Correct answer index (0–3)

**Why ScriptableObjects?**
- Easy to add or edit questions
- No code changes required
- Clean separation of data and logic

---

### ⏲️ Timer System

The timer operates in **two phases**:

| Phase | Duration | Purpose |
|-----|--------|--------|
| Answer Phase | 30 seconds | Player selects an answer |
| Reveal Phase | 10 seconds | Correct answer is shown |

#### Behavior
- Automatically advances when time expires
- Cancels early if the player answers
- Drives UI progress visuals

---

### 🧮 Score System

The ScoreKeeper tracks:
- Number of questions attempted
- Number of correct answers

Final score is calculated as:

```

(correctAnswers / totalQuestions) × 100

```

The result is displayed on the end screen.

---

### 🎮 Game Flow Control

The GameManager:
- Controls game start and end
- Manages quiz and end screen visibility
- Handles replay functionality

This keeps **scene logic clean** and avoids tight coupling.

---

## 🎨 UI & Interaction Flow

### Answer Selection Flow
1. Player clicks an answer button
2. Button sends its index to the Quiz controller
3. Quiz validates the answer
4. UI updates with correct/incorrect visuals
5. Timer switches to reveal phase
6. Next question loads automatically

UI elements are **prefab-based**, reusable, and logic-free.

---

## 🚀 Build & Release

The game has been **fully built and released** in this repository.

### 📦 Release Information
- Pre-built game binaries are available under the **GitHub Releases** section
- Users can download and play the game **without installing Unity**
- Builds are suitable for showcasing gameplay and testing

👉 **Check the Releases tab** to download the latest playable version.

This makes the repository both:
- 👨‍💻 Developer-friendly (source code)
- 🎮 User-friendly (ready-to-play build)

---

## ▶️ Running from Source

### Requirements
- Unity **6000.1.x (LTS)**
- TextMeshPro (auto-included)

### Steps
1. Clone the repository
2. Open the project in Unity
3. Load the main scene
4. Press ▶ Play

---

## 🔧 Customization & Extension

### Add New Questions
- Create a new Question ScriptableObject
- Fill in question and answers
- Assign it in the Quiz component

### Modify Gameplay
- Adjust timer durations
- Shuffle questions
- Add difficulty scaling
- Introduce categories

### Future Enhancements
- Leaderboards
- Sound effects
- Animations
- Save system
- Mobile UI support

---

## 🧪 Debugging & Common Issues

- **Timer spam in console** → Disable debug logs in Timer
- **No questions showing** → Ensure Question assets are assigned
- **Buttons not responding** → Verify OnClick bindings

---

## 🎯 Learning Outcomes

This project demonstrates:
- Clean Unity architecture
- ScriptableObject-based data modeling
- Time-driven gameplay mechanics
- UI state management
- Scalable design for small games

Ideal for:
- Unity learners
- Architecture practice
- Portfolio projects
- Technical interviews

---

## 📜 License

Open-source for educational and personal use.

---

Built using **Unity & C#**
```
