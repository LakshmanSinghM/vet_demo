# vet_demo

A simple demonstration page showing the integration of the `VET_CHAT_BOT_INTEGRATE_ANYWHERE` chatbot widget.

## Description

This repository contains a static HTML page that serves as a host for testing and demonstrating the veterinary chatbot. It simulates a veterinary clinic's website ("Paws & Claws Veterinary Clinic") where the chatbot is embedded.

## Contents

-   `index.html`: The main demo page. Includes script tags to load the chatbot and initialize user context.

## Usage

1.  **Open the file directly**:
    You can simply open `index.html` in any web browser.

2.  **Serve locally**:
    If you prefer to serve it over HTTP (recommended to avoid CORS issues with some local setups):
    ```bash
    npx serve .
    ```

## Integration Details

The demo shows how to inject context into the chatbot:

```javascript
window.VetChatbotConfig = {
    userId: "user_999",
    userName: "Alice Smith",
    petName: "Max",
    source: "demo-page"
};
```

And how to load the script:

```html
<script src="https://vet-chat-bot-integrate-anywhere.vercel.app/chatbot.js"></script>
```

*(Note: Change the `src` URL to your local build or production deployment as needed.)*
