# mcp-link Browser Extension

Welcome to the mcp-link Browser Extension! This is the core user-facing component for desktop users of the mcp-link ecosystem, acting as the secure bridge between powerful AI agents and your digital world.  It serves 2 roles:

1. It seamlessly integrates into your favorite AI chat websites, empowering them with tools you control, while ensuring you remain in command at all times.
2. It operates as a browser tool itself (when enabled and connected to a driving MCP server), allowing AI's to take actions inside your browser for you.

![mcp-link in action, showing a tool call within a chat interface](mcp-link_example_screenshot.png)

---

## 🚀 Installation

You can install the extension in two ways. The official store version is recommended for most users.

### 1. Official Store Installation (Recommended)

Get the latest stable and signed version from your browser's official store.

*   **Chrome Web Store:** *(Link coming soon)*
*   **Microsoft Edge Add-ons:** *(Link coming soon)*
*   **Firefox & Safari:** *(Support planned for a future release)*

### 2. Manual Installation (For Developers & Early Adopters)

If the store listing is not yet live or you wish to use the latest development code, you can load the extension manually.

1.  **Get the Code:** [Download the ZIP](https://github.com/AuraFriday/mcp-link/archive/refs/heads/master.zip) of this repository and extract it, or clone it using Git.
2.  **Navigate to Extensions:** In your Chromium-based browser (Chrome, Edge, Brave), open the menu (⋮) and go to `Extensions` → `Manage Extensions`.
3.  **Enable Developer Mode:** Find the "Developer mode" toggle in the top-right corner of the page and turn it on.
4.  **Load the Extension:**
    *   Click the **"Load unpacked"** button that appears.
    *   A file browser will open. Navigate to the directory where you downloaded the code and select the `extension` folder inside the main `mcp-link` directory.
    *   Click "Select folder".
5.  **Pin for Easy Access:** Click the puzzle piece icon (🧩) in your browser's toolbar and click the pin icon next to "MCP Link" to keep it visible.

---

## ⚙️ How to Use: Your First AI Tool Call

Using the extension is designed to be intuitive.

1.  **Accept the EULA:** On first use, the extension will prompt you to accept the End-User License Agreement. This is required to activate the software.
2.  **Visit a Supported AI:** Navigate to a site like `chatgpt.com` or `claude.ai`.
3.  **Chat with the AI:** The extension automatically informs the AI about the tools you have enabled. Simply ask the AI to perform a task that requires a tool.
    *   *Example prompt: "What's my current location?"*
4.  **Approve the Action:** The AI will state its intent to use a tool (e.g., `geolocation`). By default, a prompt will appear asking for your approval.
5.  **Review the Output:** The extension will display the tool's results directly in the chat interface for you and the AI to see.

---

## 🛡️ Your Security Is Our Architecture

The entire extension is built on the principle of **user consent and control.**

| Control Layer | Description |
| :--- | :--- |
| 🧩 **Tool Visibility** | **You decide what tools the AI even knows exist.** In the extension's popup menu, you can enable or disable each tool individually. If a tool is disabled, the AI has no way of knowing about it or calling it. |
| ✅ **Tool Approval** | **You approve every action.** For any enabled tool, you can set its access policy: ask for approval every time, allow it automatically for trusted tools, or run it without prompts in a sandboxed environment. |

**The AI can never take an action you have not explicitly permitted.**

### A Note on Agentic Risk & Your Responsibility

While we provide these powerful controls, it is crucial to understand the inherent risks of agentic AI.

*   **AI agents can and will make mistakes.** A command to "delete old log files" could be misinterpreted and result in the deletion of important data. An instruction to "email my team about the update" could result in sending confidential information to the wrong people.
*   **You assume all risk.** By using this software, you acknowledge that you are solely responsible for the outcomes of any action taken by an AI agent. The ultimate responsibility for any data loss, financial transaction, or other consequence rests with you, the operator.
*   **"Best-effort" is not a guarantee.** Our development dilligence, and our security review of third-party recipes in the Store is a best-effort process, not a guarantee of safety. Flaws or malicious logic may evade our notice or detection. All tools should be treated with caution and used at your own sole risk.

**We strongly recommend and expect you to take preventative measures, including maintaining regular backups of your data and utilizing sandboxed environments like Docker for executing potentially destructive tools.**

Your use of this software constitutes your explicit understanding and acceptance of these risks. The full, legally binding terms are detailed in our [End-User License Agreement](../EULA.md).

---

##  Troubleshooting & FAQ

*   **The extension icon doesn't show up in my toolbar.**
    *   Make sure you have pinned it using the puzzle piece (🧩) menu in your browser.
*   **The AI doesn't seem to know about any tools.**
    *   Click the mcp-link extension icon to open the popup. Make sure you have enabled one or more tools using the checkboxes.
*   **I see an error when loading the unpacked extension.**
    *   Ensure you have selected the correct `extension` sub-folder, not the main `mcp-link` root folder.

---

## ⚖️ Legal & Licensing

Your use of this software is governed by our End-User License Agreement. The source code is proprietary and governed by a separate license.

*   **[Read the End-User License Agreement (EULA)](../EULA.md)**
*   **[Read the Source Code License](../LICENSE)**
*   **[Read our Privacy Policy](../PRIVACY.md)**

For any issues or feature requests, please **[open an issue](../issues)** on our main project page.
