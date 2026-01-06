# QuizSphinx

A modern, interactive quiz-based learning game developed in **Unity 6** using the **Universal Render Pipeline (URP)** for 2D gameplay. This project serves as an educational tool to demonstrate game development practices including UI design, sprite management, and interactive game mechanics.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Project](#running-the-project)
- [Project Components](#project-components)
  - [Scenes](#scenes)
  - [Assets](#assets)
  - [Dependencies](#dependencies)
- [Gameplay Overview](#gameplay-overview)
- [UI/UX Design](#uiux-design)
- [Development Guidelines](#development-guidelines)
- [Contributing](#contributing)

---

## 🎮 Overview

**QuizSphinx** is a learning game development project that creates an engaging quiz experience with a polished, modern user interface. Built with **ScriptableObject-based architecture**, the game features a timed quiz system where players answer multiple-choice questions with real-time feedback. The project emphasizes clean game design patterns, effective use of Unity's rendering capabilities, and interactive gameplay mechanics. It serves as both a playable game and a reference implementation for game development best practices.

### Target Audience

- Educational players seeking interactive learning experiences
- Game developers learning Unity game development
- Students exploring 2D game mechanics and UI implementation

---

## ✨ Features

### Core Gameplay
- **Timed Quiz System**: Each question has a 30-second timer with visual progress indicator
- **Multiple-Choice Questions**: 4-option answers with instant feedback (correct/incorrect)
- **ScriptableObject Questions**: Easy question management and expansion via SO-based architecture
- **Responsive UI**: Intuitive user interface designed for accessibility
- **Visual Feedback**: Neon-themed UI elements with sprite-based feedback (correct/incorrect highlighting)
- **Answer Flow**: Show correct answer for 10 seconds before moving to next question

### Visual Design
- **Neon Aesthetic**: Modern, eye-catching neon-style graphics
- **2D Sprite-Based Graphics**: Optimized 2D rendering with URP
- **Responsive Canvas**: UI adapts seamlessly to different screen resolutions
- **Professional Color Scheme**: Dark background with vibrant accent colors (orange and blue)

### Technical Features
- **Universal Render Pipeline (URP)**: Optimized rendering for 2D games
- **TextMesh Pro Integration**: Professional text rendering and formatting
- **Modern Input System**: Support for various input devices
- **2D Animation Support**: Asset preparation for sprite animations

---

## 🛠️ Technology Stack

### Core Framework
- **Unity**: Version 6000.1.8f1 (Latest Long-Term Support)
- **Rendering**: Universal Render Pipeline (URP) 17.1.0
- **UI System**: Unity UI (UGUI) 2.0.0 & TextMesh Pro

### 2D Development
- **2D Sprites**: com.unity.2d.sprite 1.0.0
- **2D Animation**: com.unity.2d.animation 11.0.0
- **2D TileMap**: com.unity.2d.tilemap 1.0.0 & extras 4.3.1
- **Aseprite Integration**: com.unity.2d.aseprite 1.2.5
- **PSD Importer**: com.unity.2d.psdimporter 10.1.1

### Input & Scripting
- **New Input System**: com.unity.inputsystem 1.14.0
- **Visual Scripting**: com.unity.visualscripting 1.9.7
- **Timeline**: com.unity.timeline 1.8.7

### Development Tools
- **IDE Support**: Rider 3.0.36 & Visual Studio 2.0.23
- **Version Control**: Collab Proxy 2.8.2
- **Testing Framework**: Test Framework 1.5.1
- **Multiplayer Tools**: Multiplayer Center 1.0.0

---

## 📁 Project Structure

```
QuizSphinx/
├── Assets/
│   ├── Scripts/
│   │   ├── Quiz.cs                    # Main quiz controller
│   │   ├── QuestionSO.cs              # Question ScriptableObject
│   │   └── Timer.cs                   # Game timer system
│   ├── Questions/
│   │   ├── Question 1.asset           # Sample quiz question SO
│   │   ├── Question 2.asset
│   │   ├── Question 3.asset
│   │   ├── Question 4.asset
│   │   └── Question 5.asset
│   ├── Prefabs/
│   │   └── AnswerButton.prefab        # Reusable answer button UI
│   ├── Scenes/
│   │   ├── SampleScene.unity          # Main game scene
│   │   └── SampleScene.unity.meta
│   ├── Sprites/
│   │   ├── Quiz Sphinx - Gameplay Overview 1.png  # UI mockup 1
│   │   ├── Quiz Sphinx - Gameplay Overview 2.png  # UI mockup 2
│   │   ├── Quiz Sphinx - Gameplay Overview 3.png  # UI mockup 3
│   │   ├── background.png             # Background image
│   │   ├── neon_round_orange.png      # Neon UI element
│   │   ├── neon_square_blue.png       # Neon UI element
│   │   └── neon_square_orange.png     # Neon UI element
│   ├── TextMesh Pro/                  # TMP assets and resources
│   │   ├── Fonts/                     # Font files
│   │   ├── Resources/                 # TMP configuration
│   │   └── Shaders/                   # Custom text shaders
│   ├── Settings/
│   │   ├── Renderer2D.asset           # 2D renderer configuration
│   │   ├── UniversalRP.asset          # URP settings
│   │   └── Scenes/                    # Scene templates
│   ├── InputSystem_Actions.inputactions
│   ├── DefaultVolumeProfile.asset
│   └── UniversalRenderPipelineGlobalSettings.asset
├── Packages/
│   ├── manifest.json                  # Project dependencies
│   └── packages-lock.json
├── ProjectSettings/                   # Unity project configuration
└── .gitignore                         # Git ignore rules
```

---

## 🚀 Getting Started

### Prerequisites

- **Unity Hub**: Download from [unity.com](https://unity.com/download)
- **Unity Editor**: Version 6000.1.8f1 (LTS)
  - Windows 10/11 (64-bit)
  - macOS 10.13 or later
  - Linux (Ubuntu 18.04 or later)
- **Visual Studio** or **JetBrains Rider** (optional, for scripting)
- **Git**: For version control (optional)

### Installation

1. **Clone or Download the Project**
   ```bash
   git clone https://github.com/Noel-Teens/QuizSphinx
   cd "QuizSphinx"
   ```

2. **Open in Unity Hub**
   - Launch Unity Hub
   - Click "Add" → "Add project from disk"
   - Select the project folder
   - Ensure Unity 6000.1.8f1 is installed
   - Click on the project to open it

3. **Wait for Import**
   - Unity will import all assets and dependencies
   - This may take 2-5 minutes on first launch
   - Check the console for any errors

### Running the Project

1. **Open the Main Scene**
   - In the Project window, navigate to `Assets/Scenes/`
   - Double-click `SampleScene.unity` to open it

2. **Play the Game**
   - Click the **Play** button in the Unity Editor toolbar
   - The game will launch in the Game view
   - Interact with the quiz using mouse/keyboard input

3. **Build and Run**
   ```
   File → Build Settings → Select Platform → Build and Run
   ```

---

## 🎯 Project Components

### Scenes

#### SampleScene.unity
The primary game scene containing:
- **Quiz Manager**: References to Quiz.cs controller and QuestionSO data
- **Quiz UI Canvas**: Main gameplay interface with question text and 4 answer buttons
- **Timer UI**: Visual progress bar showing remaining time per question
- **Answer Buttons**: AnswerButton prefab instances (4 total) with OnClick listeners
- **Background**: Neon-themed visual backdrop
- **UI Elements**: TextMesh Pro text displays, sprite images for feedback
- **Timer Component**: Manages 30-second question timer and 10-second answer reveal timer

### Assets

#### Scripts
- **Quiz.cs**: Main quiz controller that manages question display, answer evaluation, and visual feedback
- **QuestionSO.cs**: ScriptableObject class for storing quiz questions with multiple-choice answers
- **Timer.cs**: Handles game timing with dual-phase system (question time + answer reveal time)

#### Questions (ScriptableObject Assets)
- **Question 1-5.asset**: Pre-configured quiz question assets with questions and 4-option answers
- Easily expandable by creating new QuestionSO assets in the editor

#### Prefabs
- **AnswerButton.prefab**: Reusable UI button prefab for answer options
  - Includes Image component for sprite feedback
  - Includes TextMeshProUGUI for answer text
  - Configured with Button component and OnClick event

#### Sprites
- **Quiz Sphinx Gameplay Overview**: 3 reference images showing different UI states/mockups
- **Background**: Large atmospheric background image (1080p+)
- **Neon Elements**: Decorative UI components (orange and blue variations)
  - Used for correct/incorrect answer indicators

#### TextMesh Pro
- **Fonts**: LiberationSans font with SDF rendering
- **Materials**: Drop shadow, outline, and custom text effects
- **Shaders**: Optimized text rendering shaders for various platforms

#### Settings
- **Renderer2D.asset**: 2D rendering pipeline configuration
- **UniversalRP.asset**: Global URP settings for quality and performance
- **Scene Templates**: Predefined scene setup templates

### Dependencies

All dependencies are managed via Unity Package Manager. Key packages include:

| Package | Version | Purpose |
|---------|---------|---------|
| Universal Render Pipeline | 17.1.0 | 2D/3D rendering |
| New Input System | 1.14.0 | Modern input handling |
| 2D Animation | 11.0.0 | Sprite animations |
| TextMesh Pro | - | Text rendering |
| Visual Scripting | 1.9.7 | Node-based scripting |
| Test Framework | 1.5.1 | Unit testing |

---

## 🎮 Gameplay Overview

### Typical Gameplay Flow

1. **Game Start**: Scene loads with Timer and Quiz components initialized
2. **Question Loading**: Quiz.cs loads first question from QuestionSO asset
3. **Question Display**: Question text and 4 answer options are displayed on canvas
4. **Timer Countdown**: 30-second timer begins, visual progress indicator updates via Image.fillAmount
5. **Answer Selection**: Player clicks one of the 4 answer buttons
6. **Immediate Feedback**: 
   - If correct: "Correct!" message displays, correct button highlighted with sprite change
   - If incorrect: "Sorry, the correct answer was..." message with correct answer highlighted
7. **Answer Reveal Phase**: 10-second timer displays correct answer before proceeding
8. **Next Question**: Timer resets, new question loads, buttons re-enabled and reset to default sprite
9. **Quiz Loop**: Cycle repeats with next QuestionSO asset

### Timer System Details

- **Question Timer**: 30 seconds for player to answer
- **Answer Reveal Timer**: 10 seconds to show correct answer
- **Visual Indicator**: Image component fillAmount updates based on fillFraction
- **Auto-Advance**: If no answer selected within time, correct answer auto-displays

### Visual States (Based on Gameplay Overviews)

- **Overview 1**: Initial question presentation layout with timer bar
- **Overview 2**: Alternative UI arrangement or mid-game state with active timer
- **Overview 3**: Answer feedback state or results screen

---

## 🎨 UI/UX Design

### Design Philosophy

- **Neon Aesthetic**: Modern, eye-catching visual style with high contrast
- **Accessibility**: Large, readable text using TextMesh Pro
- **Responsiveness**: UI scales properly on different screen sizes
- **Visual Feedback**: Interactive elements respond to user actions
- **Color Scheme**: Dark backgrounds with vibrant orange and blue accents

### UI Elements

- **Answer Buttons**: Neon-styled clickable options (orange/blue variations)
- **Question Display**: Prominent text area for quiz questions
- **Score Counter**: Real-time score tracking display
- **Background**: Atmospheric neon-themed backdrop

---

## 💻 Development Guidelines

### Code Style

- Use **PascalCase** for class names and public methods
- Use **camelCase** for private fields and local variables
- Add XML comments to public methods and classes
- Keep methods focused and under 30 lines when possible

### Asset Management

- Organize sprites in the `Assets/Sprites/` folder
- Use descriptive naming conventions (e.g., `neon_square_blue`)
- Keep scenes in `Assets/Scenes/` with version control
- Use nested prefabs for complex UI hierarchies

### Question Asset Creation

1. Right-click in Project window → Create → Quiz Question
2. Name the asset (e.g., "Question 6")
3. Set the question text in the TextArea field
4. Fill in 4 answer options
5. Set the correct answer index (0-3)
6. Reference in Quiz.cs or create a question manager for multiple questions

### Performance Optimization

- Profile with the Unity Profiler (Window → Analysis → Profiler)
- Minimize draw calls by batching sprites
- Use object pooling for frequently instantiated objects
- Optimize texture sizes and compression settings
- Preload QuestionSO assets to avoid load time during gameplay
- Use FixedUpdate for timer to ensure consistent timing

### Best Practices

- Test frequently during development
- Use the Scene and Game views effectively
- Keep the hierarchy organized with clear naming
- Document complex gameplay systems
- Use version control (Git) for collaboration

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. **Fork the Repository**: Create your own copy
2. **Create a Branch**: `git checkout -b feature/your-feature`
3. **Make Changes**: Implement your improvements
4. **Test Thoroughly**: Ensure no regressions
5. **Submit a Pull Request**: Describe your changes clearly

### Areas for Contribution

- Additional quiz questions (create new QuestionSO assets)
- Question categories and difficulty levels
- Score tracking and leaderboard system
- Sound effects and audio feedback
- Enhanced visual effects and animations
- Question shuffling and randomization
- Multi-round quiz mode
- Improved accessibility features
- Performance optimizations
- Documentation improvements
- Bug fixes and testing

---

## 📚 Additional Resources

- [Unity Manual - 2D](https://docs.unity3d.com/Manual/2D.html)
- [Universal Render Pipeline Documentation](https://docs.unity3d.com/Manual/universal-render-pipeline.html)
- [TextMesh Pro Documentation](https://docs.unity3d.com/Manual/TextMeshPro.html)
- [New Input System Guide](https://docs.unity3d.com/Packages/com.unity.inputsystem@latest/index.html)

---

## 🐛 Troubleshooting

### Common Issues

**Issue**: "Cannot find referenced script"
- **Solution**: Ensure all scripts are in the `Assets/` folder and reimport by pressing `Ctrl+R`

**Issue**: "Textures appear blurry"
- **Solution**: Check texture import settings - set "Filter Mode" to "Point (no filter)" for pixel-perfect rendering

**Issue**: "UI text not displaying correctly"
- **Solution**: Verify TextMesh Pro is properly installed (Window → TextMesh Pro → Import TMP Essential Resources)

**Issue**: "Game runs slowly"
- **Solution**: Use the Profiler to identify bottlenecks; check draw call count and memory usage
