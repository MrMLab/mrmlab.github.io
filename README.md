# Mr. M Portfolio

> **An interactive, AI-driven, and highly secure personal portfolio engineered for the modern web.**
> 
> 🔗 **Experience the Live AI Platform [Here!](https://mrmlab.github.io)**

![React](https://img.shields.io/badge/React-19.0-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.4-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Groq API](https://img.shields.io/badge/AI_Inference-Groq_API-f55036?style=for-the-badge)
![Security](https://img.shields.io/badge/Security-Fortified-success?style=for-the-badge&logo=security)
![License](https://img.shields.io/badge/License-Proprietary-blue?style=for-the-badge)

---

## 🚀 Executive Overview

Welcome to the **Mr. M Portfolio**—a paradigm shift in how professional identities are presented online. Moving beyond traditional static resumes, this platform introduces a fully conversational, AI-powered interface that allows professionals, recruiters, and tech enthusiasts to interact directly with a virtual representation of Marco Hadi Surya.

Designed with a sleek, cyberpunk-inspired aesthetic, the application seamlessly blends high-performance frontend engineering with state-of-the-art Large Language Model (LLM) inference. It doesn't just list skills and experiences; it actively engages users, answers contextual questions, and fetches real-time data to provide an immersive and highly personalized user experience. Furthermore, the application is wrapped in a robust, military-grade client-side security layer to prevent reverse engineering and unauthorized tampering.

## ✨ Key Features & Advantages

*   **Conversational AI Interface:** Replaces static text with a dynamic chat interface powered by ultra-fast LLM inference. Users can naturally ask about skills, experiences, and contact information.
*   **Real-Time Data Injection (RAG-lite):** Intelligently detects user intent. When queried about "projects," the system autonomously fetches live data and README summaries directly from GitHub repositories, injecting them into the AI's context window for accurate, up-to-date responses.
*   **Advanced Operational Security (OPSEC):** Implements a tamper-evident execution environment. Features include DevTools trapping, strict Content Security Policies (CSP), execution timing checks, and dynamic fetch-overriding to thwart debugging and unauthorized data scraping.
*   **Intelligent Session Persistence:** Utilizes local storage to maintain chat history. If a user accidentally closes the tab, a sleek modal detects the previous session and offers a seamless resumption of the conversation.
*   **Immersive Cyberpunk UX/UI:** Features a custom HTML5 Canvas particle network background, typewriter text effects, scanline overlays, and a highly responsive layout optimized for both desktop and mobile environments.

## 🏗️ High-Level Architecture

The system is designed as a secure, single-page application (SPA) with a highly modular data flow. The architecture operates entirely on the client side while securely orchestrating external API communications.

### 1. The Security & Environment Layer
Before the main application initializes, a strict security daemon runs in the background. It monitors window dimensions, keystrokes, and execution latency. If anomalous behavior (such as opening browser developer tools) is detected, the application immediately halts execution and renders a decoy 404 page, ensuring the proprietary logic remains unexposed.

### 2. The Interceptor & Context Middleware
At the core of the application is a custom network interceptor. Instead of directly calling the AI endpoint, all outgoing requests pass through this middleware:
*   **Persona Retrieval:** On load, the system fetches a proprietary system prompt (persona) from a secure external source.
*   **Intent Routing:** When a user submits a query, the middleware analyzes the text. If it detects keywords related to portfolio projects, it triggers a parallel asynchronous pipeline.
*   **Dynamic Context Assembly:** The pipeline fetches real-time repository data, parses it, and injects it as a hidden system alert into the payload. This ensures the AI has the latest factual data without hardcoding it into the application.

### 3. The Inference Engine
The assembled context (Persona + Real-time Data + Chat History + User Query) is securely transmitted to the **Groq API**. The system dynamically selects the most optimal and fastest available model for inference, ensuring near-instantaneous response times.

### 4. The Presentation Layer
The response is streamed back to the React-based UI. A custom rendering engine parses the markdown-lite response and displays it using a typewriter effect, creating a natural, human-like conversational cadence.

## 🛠️ Tech Stack

**Frontend & UI:**
*   **React.js (v19):** Core UI library for reactive state management and component rendering.
*   **Tailwind CSS:** Utility-first styling for the responsive, cyberpunk-themed interface.
*   **HTML5 Canvas & Vanilla JS:** For lightweight, high-performance background particle animations.
*   **Lucide Icons:** Scalable vector graphics for intuitive UI navigation.

**Data Pipeline & AI:**
*   **Groq API:** High-speed LLM inference engine for natural language processing.
*   **GitHub REST API:** For real-time repository and README data extraction.
*   **Custom Fetch Interceptor:** Proprietary middleware for dynamic prompt engineering and intent routing.

**Security & Infrastructure:**
*   **Strict Content Security Policy (CSP):** Mitigates XSS and unauthorized resource loading.
*   **Anti-Debugging Scripts:** Custom timing and environment checks to prevent reverse engineering.
*   **Vite/Rollup:** For aggressive code minification and bundling.

---

## ⚖️ Copyright & License

**© Mr. M. All rights reserved.**

*This software and its underlying architecture are proprietary. Unauthorized copying, reverse engineering, distributing, or modifying of the source code, via any medium, is strictly prohibited.*

**Interested in the source code or a custom implementation?**  
For business inquiries, collaborations, or source code requests, please reach out via the contact channels available directly on my **[Portfolio Website](https://mrmlab.github.io)**.
