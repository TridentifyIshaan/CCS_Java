![header](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=7)

# Customer Care Simulation for Vistara Airlines

## Overview
The **Customer Care Simulation for Vistara Airlines** is a text-to-speech simulation of customer care for Vistara Airlines.

This project will simulate an IVR (Interactive Voice Response) system where a user navigates through different options, just like when calling customer support.

## Features
**Text-to-Speech (TTS) Support**
- Uses FreeTTS to convert text to speech for user interaction.
- Provides voice output for English and Hindi options.

**Multilingual Support**

- Users can select English or Hindi for interaction.
- Uses predefined prompts and responses for both languages.

**Interactive Voice Menu**
- Users can choose:
-> Flight status (Randomized on-time/delay/cancel status).
-> Flight cancellation request (Takes PNR and flight number).
-> Customer support (Simulated wait message).

**Randomized Flight Status**
- Uses Random class to generate different flight statuses.

**Terminal-Based Execution**
- Works as a console-based application that is suitable for kiosks, IVR-like systems, or simple automation.

## Architecture
The project follows a modular design:
- **Input Handling:** Uses Scanner to take user input (numeric choices, PNR, flight number).
- **Text-to-Speech Engine:** Uses FreeTTS (Java-based speech synthesis), initializes VoiceManager & Voice (kevin16 voice) and calls speak() method for text output in speech.
- **Menu Selection & Processing:** Uses a switch statement to handle user choices and calls speak() and System.out.println() for both audio & text output.
- **Error Handling & Cleanup:** Uses try-catch-finally for handling NullPointerException (if voice engine fails) and ensures voice.deallocate() & input.close() to free resources.

## Project Structure
```bash
app/
├── build.gradle
├── src/
│   ├── main/
│   │   └── java/
│   │       └── customercaresimulation/
│   │           └── App.java
│   └── test/
│       └── java/
│           └── customercaresimulation/
│               └── AppTest.java
└── libs/
```

## Prerequisites
- Java 8+ ( For Backend )
- APIs:
  - FreeTTS API

## Overall Tech Stack

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
  
## License
This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International Public License. See the [LICENSE](https://github.com/TridentifyIshaan/VaayuNetra/blob/cca180278d1da7978c79f5a6b1bf966a93410ce9/LICENSE) file for details.

### 🐈‍⬛ GitHub Profiles of Creators:

[![GitHub Ishaan Rastogi](https://img.shields.io/badge/IshaanRastogi-%23FFFFFF.svg?logo=GitHub&logoColor=black)](https://github.com/TridentifyIshaan)

### ✍️ Random Dev Quote
![](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical)
