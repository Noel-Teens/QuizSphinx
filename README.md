# Quiz Sphinx

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
- [License](#license)

---

## 🎮 Overview

**Quiz Sphinx** is a learning game development project that creates an engaging quiz experience with a polished, modern user interface. The project emphasizes clean game design patterns, effective use of Unity's rendering capabilities, and interactive gameplay mechanics. It serves as both a playable game and a reference implementation for game development best practices.

### Target Audience

- Educational players seeking interactive learning experiences
- Game developers learning Unity game development
- Students exploring 2D game mechanics and UI implementation

---

## ✨ Features

### Core Gameplay
- **Interactive Quiz Mechanics**: Engaging multiple-choice quiz system with visual feedback
- **Score Tracking**: Real-time score updates and performance metrics
- **Responsive UI**: Intuitive user interface designed for accessibility
- **Visual Feedback**: Neon-themed UI elements with smooth animations and transitions

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
Quiz Sphinx/
├── Assets/
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
- **Quiz UI Canvas**: Main gameplay interface with quiz questions and answer options
- **Background**: Neon-themed visual backdrop
- **UI Elements**: Buttons, text displays, and visual feedback systems
- **Input Handlers**: Manages player interactions

### Assets

#### Sprites
- **Quiz Sphinx Gameplay Overview**: 3 reference images showing different UI states/mockups
- **Background**: Large atmospheric background image (1080p+)
- **Neon Elements**: Decorative UI components (orange and blue variations)

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

1. **Game Start**: Player enters the main quiz scene
2. **Question Display**: A quiz question appears with visual styling
3. **Answer Selection**: Player clicks on one of the multiple-choice options
4. **Feedback**: Visual and/or audio feedback indicates correct/incorrect answer
5. **Score Update**: Score is updated in real-time
6. **Next Question**: Game transitions to the next question
7. **Quiz End**: Final score is displayed with performance summary

### Visual States (Based on Gameplay Overviews)

- **Overview 1**: Initial question presentation layout
- **Overview 2**: Alternative UI arrangement or mid-game state
- **Overview 3**: Results or summary screen

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

### Performance Optimization

- Profile with the Unity Profiler (Window → Analysis → Profiler)
- Minimize draw calls by batching sprites
- Use object pooling for frequently instantiated objects
- Optimize texture sizes and compression settings

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

- Additional quiz questions and categories
- Enhanced visual effects and animations
- Improved accessibility features
- Performance optimizations
- Documentation improvements
- Bug fixes and testing

---

## 📝 License

This project is provided for educational purposes. Please refer to the LICENSE file for specific terms and conditions.

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
