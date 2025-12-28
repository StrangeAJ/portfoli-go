---
title: "GoCyberChef"
date: 2025-10-18
description: "A high-performance, progressive web app (PWA) version of the popular CyberChef security tool, built with Go and WebAssembly."
tech: ["Go", "WebAssembly", "PWA", "JavaScript"]
source: "https://github.com/StrangeAJ/GoCyberChef"
live: "https://cyberchef.ashishjingar.in"
---

## Overview

GoCyberChef is a modern reimagining of the popular CyberChef utility, built from the ground up in Go and compiled to WebAssembly (WASM). The goal is to create a blazing-fast, client-side Progressive Web App (PWA) for data manipulation and analysis that can be used online or offline by security professionals.

### Key Features
- **High Performance**: Leverages the speed of Go and WebAssembly for near-native performance on complex data operations.
- **Offline Capability**: As a PWA, it's installable and works entirely offline, ensuring tools are always available.
- **Client-Side Security**: All operations run directly in the browser, meaning sensitive data never leaves your machine.
- **Modular Interface**: Retains the familiar, recipe-based interface for chaining together various data operations.

### Technical Implementation
- **Core Logic**: Written entirely in Go for performance and type safety.
- **Frontend**: Compiled to WebAssembly to run in the browser, with a lightweight JavaScript wrapper for DOM interaction.
- **PWA Functionality**: Implemented using Service Workers and a Web App Manifest to provide offline access and installability.

### Challenges & Solutions
- **Challenge**: Efficiently manipulating the browser's DOM from Go code compiled to WASM.
  - **Solution**: Utilized Go's `syscall/js` package to create bindings that allow Go to call JavaScript functions and interact with web APIs.
- **Challenge**: Maintaining a responsive UI during heavy, synchronous data processing.
  - **Solution**: Structured complex operations to run in web workers where possible to prevent blocking the main browser thread.