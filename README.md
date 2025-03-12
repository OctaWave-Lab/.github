# **OctaWave Lab - Audio Processing Solutions**
Welcome to **OctaWave Lab**, This is the pet-project I created for fun and educational purposes. It ain't perfect, never was and will never be. The Main idea is simple: to create guitar tuner using KMP and C++. More details is below. GL & HF.

---

## 🎯 **Project Idea**
The goal of **OctaWave Lab** is to develop a cross-platform solution that combines the simplicity of Kotlin for UI and app logic with the performance of C++ for intensive audio processing tasks.

### **Core Use Case**
- The user records or uploads an audio file.
- The C++ library processes the data using FFT.
- The system identifies and returns the dominant frequency in the audio sample.

This architecture ensures flexibility, scalability, and the ability to extend functionality with additional audio analysis features in the future.

---

## 📁 **Project Structure**
```
OctaWave Lab
├── OctaWave-KMP          # KMP-based cross-platform project
│   ├── commonMain        # Shared code (business logic, UI logic)
│   ├── androidMain       # Android-specific implementation (JNI integration)
│   ├── iosMain           # iOS-specific implementation
│   └── composeApp        # UI implementation using Jetpack Compose
│
├── OctaWave-Processor    # C++ library for audio processing
│   ├── src               # Core processing logic (FFT, frequency detection)
│   ├── include           # Header files
│   └── CMakeLists.txt    # Build configuration
│
└── .github               # Organization profile and README file
```

---

## ⚙️ **Current Status**
✅ Core architecture established  
✅ Audio recording implemented  
✅ Audio file processing integrated  
🚧 Ongoing improvements for improved performance and feature expansion  

---

## 🔥 **Future Plans**
- Enhance the frequency detection algorithm for improved precision
- Add support for real-time audio visualization
- Introduce advanced noise reduction algorithms
- Develop additional UI features for enhanced user experience

---

## 🤝 **Contributing**
We're open to contributions! Whether you're an experienced developer or a beginner, your ideas and improvements are welcome.

1. Fork the repository
2. Create a new branch for your feature
3. Submit a pull request

---

## 🚀 **Project Overview**
Our system is built as a cross-platform solution with two primary projects:

### 1. **OctaWave-KMP**
**Kotlin Multiplatform Project (KMP)** — The main application that integrates audio processing features using native code.

- **Purpose:** Provides the user interface, audio recording functionality, and handles interactions with the C++ audio processing library.
- **Architecture:** Utilizes **MVVM** for clear separation of concerns and scalability.
- **Technology Stack:**
  - **Kotlin Multiplatform (KMP)** for cross-platform logic
  - **Jetpack Compose** for UI
  - **C++ (via JNI)** for audio processing logic
  - **CMake** for native code integration
- **Key Features:**
  - Real-time audio recording and playback
  - File-based audio processing
  - Communicates with the C++ library for efficient audio analysis

---

### 2. **OctaWave-Processor**
**C++ Audio Processing Library** — A core library built to efficiently analyze audio data and detect dominant frequencies.

- **Purpose:** Provides the core audio processing logic using FFT (Fast Fourier Transform) for accurate frequency detection.
- **Architecture:** Modular design with reusable components for future expansions.
- **Technology Stack:**
  - **C++17** for performance
  - **FFT Algorithm** for audio analysis
  - **CMake** for project building and integration
- **Key Features:**
  - Fast and accurate frequency detection
  - Optimized for low-latency processing
  - Designed to be reusable in different platforms via JNI or other interfaces

---

## 📩 **Contact**
For questions, suggestions, or collaboration inquiries, feel free to reach out via **GitHub Discussions** or directly contact the maintainers.

Let's build the future of audio processing together! 🚀
