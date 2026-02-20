# 🤖 Nexus AI: A Full-Stack ChatGPT Clone

A high-performance, real-time conversational AI platform. **Nexus AI** replicates the core experience of ChatGPT, featuring fluid streaming responses, categorized chat history, and seamless cross-device synchronization.

## ⚡ The Experience

Nexus AI isn't just a wrapper; it's a complete ecosystem. By combining the conversational depth of **Google Gemini** with the real-time infrastructure of **Firebase**, this clone offers a zero-latency feel with enterprise-grade data persistence.

## ✨ Key Features

* **Streaming Responses:** Watch the AI "type" in real-time using Server-Sent Events (SSE) or Firebase triggers.
* **Persistent Chat History:** All conversations are indexed and stored in **Firestore**, allowing you to pick up exactly where you left off.
* **Smart Title Generation:** Google AI automatically generates a concise title for your chat based on the first few messages.
* **Markdown Support:** Full rendering for code blocks (with syntax highlighting), tables, and mathematical formatting.
* **Multi-Modal Ready:** Upload images to the chat and ask the AI to describe, analyze, or code them (powered by Gemini Vision).
* **Secure Auth:** Google and Email/Password sign-in via **Firebase Authentication**.

## 🛠️ Tech Stack

* **AI Engine:** [Google Gemini API](https://ai.google.dev/) (The "Brain")
* **Platform:** [Firebase Studio](https://firebase.google.com/)
* **Firestore:** For real-time chat document storage.
* **Hosting:** Globally distributed edge hosting.
* **Functions:** To securely handle API keys and AI logic.


* **Frontend:** [Insert Framework, e.g., Next.js / React]
* **Styling:** [e.g., Tailwind CSS / Headless UI]

## 🚀 Quick Start

### 1. Prerequisites

* Node.js (v18+)
* A Firebase Project
* A Google AI Studio API Key

### 2. Installation

```bash
git clone https://github.com/your-username/nexus-ai-clone.git
cd nexus-ai-clone
npm install

```

### 3. Environment Variables

Create a `.env.local` file:

```env
NEXT_PUBLIC_FIREBASE_API_KEY=your_key
GOOGLE_AI_API_KEY=your_gemini_api_key

```

### 4. Deployment

Deploy to Firebase with a single command:

```bash
firebase deploy

```

## 📂 Database Schema (Firestore)

```text
users/
  └── {userId}/
      └── chats/
          └── {chatId}/
              ├── metadata (title, timestamp, model)
              └── messages/
                  └── {messageId} (role, content, timestamp)

```

## 🛠️ Roadmap

* [ ] **System Prompts:** Allow users to define "Personas" (e.g., Creative Writer, Senior Coder).
* [ ] **Voice Mode:** Integration with Web Speech API for hands-free chatting.
* [ ] **Search:** Full-text search across all historical conversations.

---

**Built to demonstrate the power of Modern AI and Cloud Serverless Architecture.**
