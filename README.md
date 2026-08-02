# Baybayin v2026 - Filipino Script Learning App 2026

> **Baybayin is a browser-based Filipino script study tool for version 2026, combining flashcards, quizzes, and progress tracking to make writing-system practice more engaging.**

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/cbraun64/baybayin-script-study-app?style=flat-square)](https://github.com/cbraun64/baybayin-script-study-app)

---

<p align="center">
  <a href="https://cbraun64.github.io/baybayin-script-study-app/">
    <img src="https://img.shields.io/badge/Download-Baybayin%20Latest-brightgreen?style=for-the-badge" alt="Download Baybayin">
  </a>
</p>

> **[Download Baybayin v2026](https://cbraun64.github.io/baybayin-script-study-app/)**

---

[Download Latest Build](https://cbraun64.github.io/baybayin-script-study-app/)

---

## What Is Baybayin?

Baybayin is a static web application built around interactive practice for the Baybayin script. Its learning flow combines character flashcards, multiple-choice challenges, and review features, allowing learners to work on recognition and recall in the same app.

It can support classroom learners, independent study, and users refreshing their knowledge of Filipino writing systems. Practice is available as a local guest session, while Firebase integration provides a cloud-connected option for users who want synchronized progress.

---

## Highlights

- Revisit characters through repeatable flashcard sessions
- Test recognition with multiple-choice questions
- Practice difficult characters through missed-item review
- Keep guest progress locally with `localStorage`
- Synchronize connected-session data using Firebase Firestore
- Sign in to connected accounts with Google
- Track sessions with streak, combo, and heart mechanics
- Hear speech output with romanization used as a fallback
- Browse a character chart with glyph and reading views

---

## Getting Started

Because Baybayin is distributed as a static site, it does not require a complex installation process.

1. Clone the repository or download its files:
   - `git clone https://github.com/cbraun64/baybayin-script-study-app.git
2. Change into the project directory.
3. Serve the files through a static web server or deploy them to a hosting service.
4. For local development, open the primary HTML entry file in a browser or launch a lightweight development server.

To start a local preview, run:

- `python -m http.server 8000`

Open `http://localhost:8000` in your browser.

---

## Using the App

Flashcards are a good starting point for learning glyphs and readings. Once you are familiar with the material, use the quiz to measure how well you can recall it.

A normal study session looks like this:

1. Select guest mode for browser-only practice, or use Google sign-in when you want progress synchronization.
2. Review characters with flashcards.
3. Challenge yourself with the multiple-choice quiz.
4. Revisit the characters you missed.
5. Consult the character chart to compare glyphs and readings.
6. Practice consistently to develop streaks and preserve progress.

To use spoken learning support, turn on speech features in a browser with speech synthesis support.

---

## Configuration

Guest sessions keep settings and progress in the browser. Sessions connected to an account use Firebase services for cloud functionality.

A sample application configuration is shown below:

    firebaseConfig:
      apiKey: your-api-key
      authDomain: your-auth-domain
      projectId: your-project-id
      appId: your-app-id

The browser manages local session information through `localStorage`. When sign-in is configured, Firebase Firestore handles cloud synchronization.

---

## Requirements

- A current web browser
- HTML support for hosting a static website
- JavaScript enabled in the browser
- An optional Firebase project for cloud synchronization
- Optional Google sign-in configuration for authenticated use
- Speech synthesis support in the browser for voice output

---

## Frequently Asked Questions

**How can I update Baybayin?**  
Download the newest build from the project page, then replace the files currently being hosted.

**Is an account required?**  
No. Guest mode lets you practice without signing in and stores progress in the browser.

**Where does the app save my progress?**  
Guest sessions use `localStorage`. When you are signed in, progress may synchronize through Firebase Firestore.

**Why is there no audio?**  
Check that your browser supports speech synthesis and verify that browser settings are not preventing sound playback.

**What can I do about synchronization problems?**  
Review your Firebase configuration and make sure Google sign-in has been enabled for the Firebase project.

---

## Planned Improvements

- Provide additional ways to move through practice sessions
- Strengthen the study and review experience
- Offer more feedback for missed characters
- Continue improving learning interactions on mobile devices

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
