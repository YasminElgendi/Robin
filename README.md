# Robin 

### ML-Powered Voice Programming Assistant

**Robin** is an AI-powered voice programming assistant designed to make software development more accessible by enabling users to interact with their development environment through voice commands and hands-free controls.

The project was developed as a graduation project with a focus on **accessibility, machine learning, natural language processing, speech interaction, and developer productivity**.

---

## 🎯 Motivation

Traditional programming environments rely heavily on keyboards and mice, which can create significant barriers for people with limited mobility or visual impairments.

Robin aims to reduce this dependency by allowing users to perform common programming and computer interactions through natural voice commands.

Instead of requiring users to memorize rigid command phrases or dictate entire programs, Robin understands the **intent behind spoken commands** and translates them into appropriate actions.

---

## ✨ Key Features

### 🗣️ Natural Language Command Recognition

Robin uses an NLP-based intent recognition system to understand different ways of expressing the same command.

The command-processing pipeline includes:

* Text preprocessing
* TF-IDF feature extraction
* N-gram features
* Multiclass Logistic Regression
* One-vs-Rest classification

The trained model achieved approximately **98% test accuracy** on the project's command-intent dataset.

---

### ⚙️ Command Execution

Recognized commands are translated into actions within the user's development environment.

Robin can interact with:

* Files and folders
* Source code
* Development tools
* IDE operations
* System-level actions

This allows users to perform programming-related tasks without relying entirely on traditional input devices.

---

### 🎙️ Voice Interaction

Robin provides a voice-driven interface that allows users to interact with the assistant naturally.

The system supports:

* Speech recognition
* Voice commands
* Text-to-speech feedback
* Interactive voice-based workflows

---

### 💻 Interactive Programming Mode

Robin includes an interactive mode designed to make coding through voice more practical.

It provides:

* Voice-driven programming interactions
* Code-related feedback
* Code summaries
* VS Code diagnostic feedback
* Text-to-speech responses

---

### 🖱️ Head-Tracking Mouse Control

Robin also includes a computer-vision-based head-tracking system that allows users to control the mouse using head movements.

This provides an additional hands-free interaction method beyond voice commands.

---

## 🧠 System Architecture

Robin is composed of several interconnected modules:

```text
                    ┌─────────────────────┐
                    │      User Input     │
                    │   Voice / Head      │
                    │     Movement        │
                    └──────────┬──────────┘
                               │
              ┌────────────────┴────────────────┐
              │                                 │
              ▼                                 ▼
     ┌─────────────────┐              ┌─────────────────┐
     │ Speech          │              │ Mouse Tracking  │
     │ Recognition     │              │ Computer Vision │
     └────────┬────────┘              └────────┬────────┘
              │                                 │
              ▼                                 │
     ┌─────────────────┐                        │
     │ Command Intent  │                        │
     │ Recognition     │                        │
     └────────┬────────┘                        │
              │                                 │
              ▼                                 │
     ┌─────────────────┐                        │
     │ Command         │◄───────────────────────┘
     │ Execution       │
     └────────┬────────┘
              │
              ▼
     ┌─────────────────┐
     │ Development     │
     │ Environment     │
     └─────────────────┘
```

---

## 🛠️ Technologies

| Area             | Technologies                        |
| ---------------- | ----------------------------------- |
| Machine Learning | Scikit-learn, Logistic Regression   |
| NLP              | TF-IDF, N-grams, Text Preprocessing |
| Speech           | Speech Recognition, pyttsx3         |
| Computer Vision  | OpenCV                              |
| Programming      | Python                              |
| IDE Integration  | Visual Studio Code                  |
| Code Parsing     | Tree-sitter                         |
| Architecture     | Modular Python components           |

---

## 📁 Project Structure

```text
Robin/
│
├── CommandExecution/    # Executes recognized commands
├── CommandIntent/       # NLP-based intent recognition
├── DesktopApplication/  # Main desktop application
├── InteractiveMode/     # Interactive coding experience
├── MouseTracking/       # Head-tracking mouse control
├── SpeechRecognition/   # Speech processing
├── Assets/              # Project assets
├── Thesis/              # Project documentation and diagrams
│
└── README.md
```

---

## 🚀 How It Works

A typical interaction follows this pipeline:

1. The user speaks a command.
2. Robin converts the speech into text.
3. The NLP pipeline preprocesses the text.
4. The intent classification model determines what the user wants to do.
5. The corresponding command is executed.
6. Robin provides feedback through voice or the development environment.

For example:

```text
User:
"Create a new Python file"

        ↓

Speech Recognition

        ↓

"create a new python file"

        ↓

Intent Recognition

        ↓

CREATE_FILE

        ↓

Command Execution

        ↓

New Python file created
```

---

## ♿ Accessibility

Accessibility is at the core of Robin's design.

The project explores multiple ways of reducing dependency on traditional computer input:

* Voice-based programming
* Voice-driven IDE interaction
* Head-tracking mouse control
* Text-to-speech feedback
* Natural-language commands

The goal is not simply to automate programming tasks, but to make existing development workflows more accessible.

---

## 📊 Machine Learning Performance

The command-intent classification model achieved approximately:

**98% test accuracy**

The model was trained to classify natural-language commands into predefined intents using TF-IDF and n-gram features with a multiclass Logistic Regression classifier.

---

## 👩‍💻 My Contribution

Robin was developed as a team graduation project.

My contributions included:

* Designing and implementing the NLP intent-recognition pipeline
* Text preprocessing and feature extraction
* Training and evaluating the intent classification model
* Implementing command execution logic
* Integrating voice interaction with development tools
* Contributing to the overall system architecture
* Working on the integration between the project's AI components and the development environment

---

## 🎓 Project Context

**Graduation Project — Computer Engineering**

Robin was developed as a practical exploration of how machine learning, natural language processing, speech technologies, and computer vision can be combined to create a more accessible programming experience.

The project received a **Distinction**.

---

## 📌 Future Improvements

Potential future improvements include:

* Supporting more programming languages and IDEs
* Improving natural-language understanding with modern transformer-based models
* Adding personalized command learning
* Improving speech recognition for different accents and noisy environments
* Expanding accessibility features
* Adding more advanced AI-assisted coding capabilities

---

## 📄 Documentation

Additional project documentation, diagrams, and research material can be found in the [`Thesis/Diagrams`](./Thesis/Diagrams) directory.

---

## 👥 Team

Robin was developed as a collaborative graduation project by a team of four Computer Engineering students.

---

**Robin — Making programming more accessible, one command at a time.**
