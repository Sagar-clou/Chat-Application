# Orbit Chat — Responsive Chat UI

A polished, teal-accented, responsive chat-interface demo built with plain HTML, CSS, and JavaScript. It is based on the supplied `new.html` and fixes the broken JavaScript so the interface can be used locally.

## Features

- Responsive layout for desktop, tablet, and mobile screens
- Contact list with conversation filtering
- Switch between sample conversations
- Send messages and display timestamps
- `Enter` sends a message; `Shift + Enter` inserts a new line
- Local message history using browser `localStorage`
- Clear locally saved chat history
- Accessible labels, keyboard contact selection, and reduced-motion support
- No build step or package installation required

## Run it

1. Keep `new.html` in a folder.
2. Open `new.html` in a modern browser (Chrome, Edge, Firefox, or Safari).
3. Select a contact, type a message, and press **Enter** or the send button.

You can also serve the folder locally, for example:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000/new.html`.

## Important limitation

This is a **front-end demo only**. It does not connect to a WebSocket server, authenticate users, or send messages to other devices. The contacts and initial messages are sample content; messages you send are stored only in the current browser's local storage. The avatar images use remote URLs and may require an internet connection.

## Files

- `new.html` — complete application (HTML, CSS, and JavaScript)
- `README.md` — project overview and run instructions

## Technology

- HTML5
- CSS3 (responsive grid/flex layouts, custom properties, media queries)
- Vanilla JavaScript
- Browser `localStorage`

## Next steps for a real chat application

To make this a real-time multi-user chat, add a WebSocket backend (for example, Node.js with `ws` or Socket.IO), user authentication, server-side message validation, persistent database storage, and appropriate transport security (HTTPS/WSS). Never treat a front-end status label as proof of a real server connection.
