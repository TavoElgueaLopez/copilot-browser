# 🤖 GitHub Copilot Integration Guide

## 🚀 How It Works (Zero Config)

We have designed this to be "Plug and Play". You do **NOT** need to install Node.js or run any servers manually.

### The Architecture
1.  **VS Code Extension**:
    -   Contains the **Embedded Relay Server**.
    -   Automatically starts the server on port `8080` when VS Code opens.
2.  **Chrome Extension**:
    -   Connects to that local server (`ws://localhost:8080`).
3.  **GitHub Copilot**:
    -   Talks to the VS Code Extension to send commands.

---

## 📦 Setup Guide

### Step 1: Install Chrome Extension
1.  Download `browser-extension.zip` (or install from Web Store).
2.  Go to `chrome://extensions/`.
3.  Enable **Developer Mode** (top right).
4.  Drag and drop the folder/zip to install.
5.  **Status**: The icon should turn green ✅ when VS Code is open.

### Step 2: Install VS Code Extension
1.  Install **Copilot Browser Connector** from the Marketplace.
2.  Open your project in VS Code.
3.  **That's it!** The server starts automatically. 
    -   *Check the status bar: "Browser: Connected"*

---

## 💬 How to Use with Copilot

You don't need to run code. Just **chat** with Copilot.

### 1. Ask Copilot to Perform Actions
> "Navigate to google.com and search for 'VS Code'"

### 2. Ask for Information
> "Get the console logs from this page"
> "What is the text inside the clean button?"

### 3. Debugging
> "Take a screenshot and tell me if the layout looks broken"

## 🔧 Troubleshooting

-   **"Browser: Disconnected"**:
    -   Ensure Chrome is open.
    -   Ensure the Chrome Extension is enabled.
    -   Refresh the web page.

-   **"Command not found"**:
    -   Make sure you installed the specific **Copilot Browser Connector** extension.
