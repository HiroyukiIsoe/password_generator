# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a secure password generator web application built with vanilla HTML, CSS, and JavaScript. The project implements a client-side password generator with advanced security features and an intuitive user interface.

## Project Architecture

- **Technology Stack**: Vanilla HTML5, CSS3, JavaScript (ES6+)
- **No Build System**: Direct browser execution, no compilation required
- **No Dependencies**: Self-contained implementation using only web standards

## Current Implementation

### File Structure
```
public/
├── index.html      # Main HTML structure and UI elements
├── styles.css      # Complete styling with responsive design
└── script.js       # Password generation logic and UI interactions
docs/
└── design.md       # Requirements specification (Japanese)
```

### Key Features Implemented
- **Password Length Control**: 8-32 characters via slider UI
- **Character Type Selection**: Uppercase, lowercase, numbers, symbols
- **Secure Random Generation**: Uses `crypto.getRandomValues()` for cryptographic security
- **Password Strength Indicator**: Visual strength assessment (weak → very safe)
- **Clipboard Integration**: One-click copy with user feedback
- **Responsive Design**: Mobile-friendly interface
- **Input Validation**: Ensures at least one character type is selected

### Security Implementation
- Uses `window.crypto.getRandomValues()` instead of `Math.random()` for secure randomness
- Ensures all selected character types are included in generated passwords
- Implements Fisher-Yates shuffle algorithm for password character distribution

## Usage Instructions

1. **Local Development**: Open `public/index.html` directly in any modern web browser
2. **No Server Required**: All functionality works client-side
3. **No Installation**: No npm install or build process needed

## Code Standards

- **ES6+ JavaScript**: Modern JavaScript features and class-based architecture
- **Semantic HTML**: Proper markup structure and accessibility considerations
- **CSS Grid/Flexbox**: Modern layout techniques
- **Mobile-First**: Responsive design approach