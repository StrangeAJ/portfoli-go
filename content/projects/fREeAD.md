---
title: "fREeAD"
date: 2025-10-18
description: "A modern Flutter RSS reader with Material 3 design and AI-powered summarization features."
tech: ["Flutter", "Dart", "AI", "OpenAI API", "Gemini API", "Claude API"]
source: "https://github.com/StrangeAJ/fREeAD"
live: "https://github.com/StrangeAJ/fREeAD/releases/tag/Release"
---

## Overview

fREeAD is a modern, AI-enhanced RSS reader application built with Flutter. It focuses on providing a clean, customizable reading experience with intelligent features, including multi-provider AI summarization to help users quickly digest content.

### Key Features
- **Material 3 Design**: A beautiful and responsive UI that adheres to the latest Material Design principles.
- **OPML Import/Export**: Easily migrate feeds from other RSS readers.
- **AI Summarization**: Get concise summaries of articles using multiple AI providers (OpenAI, Gemini, Perplexity, Claude).
- **Bring Your Own API Key (BYOK)**: Users can securely add their own API keys to power the AI features, ensuring privacy and control.

### Technical Implementation
- **Frontend**: Developed using Flutter and Dart for a consistent experience across Android, iOS, and desktop.
- **AI Integration**: Implemented a service layer to handle REST API calls to various AI providers.
- **State Management**: Using a robust state management solution (e.g., BLoC) to handle app state efficiently.
- **Secure Storage**: User API keys are stored securely on the device using the `flutter_secure_storage` package.

### Challenges & Solutions
- **Challenge**: Integrating multiple AI APIs, each with different request/response structures.
  - **Solution**: Designed an abstraction layer (Adapter Pattern) to create a unified interface for all AI services, making it easy to switch between providers.
- **Challenge**: Ensuring user data, especially API keys, is stored securely.
  - **Solution**: Leveraged platform-specific keystores (Keychain for iOS, Keystore for Android) via `flutter_secure_storage` to encrypt and protect sensitive data.