# FloatChat  
---

**FloatChat** is a browser-based real-time chat interface designed to offer a smooth, minimal, and engaging messaging experience.  
Built originally for frontend prototyping and hackathon demos — FloatChat showcases how clean UI + auto-auth simulation can demonstrate a real-world chat flow without backend dependencies.

---

## Why FloatChat  
---

Most chat demos are either too technical or lack visual polish.  
**FloatChat** makes it simple, lightweight, and aesthetically modern.

- **Auto-filled credentials** for instant access  
- **Responsive and clean UI**  
- **Smooth chat interface simulation**  
- **Easy to extend** with real backend or APIs  

---

## Key Features  
---

| Feature | Description |
|----------|-------------|
| Instant Login | Auto-filled username and password for demo flow |
| Chat Interface | Minimal chat window UI, styled for readability |
| Responsive Layout | Works seamlessly across desktop and mobile |
| Sidebar & User Cards | Demo-ready for multi-user chat setup |
| Clean Aesthetic | Tailwind CSS-based smooth gradients and rounded UI |
| Static Frontend | No backend required — runs entirely in browser |

---

## Architecture Overview  
---

All logic runs client-side using plain **HTML, CSS, and JavaScript**.

When a user logs in:
1. Pre-filled credentials simulate instant sign-in  
2. User is redirected to the chat dashboard  
3. Messages are displayed dynamically within the same session  
4. (Optional) You can connect a backend or Firebase for real-time chat persistence  

---

## Tech Stack  
---

| Layer | Technology |
|--------|-------------|
| Frontend | HTML5, CSS3, JavaScript |
| Styling | Tailwind CSS |
| UI Components | Custom cards, sidebar layout |
| Icons | Lucide / Remix icons |
| Deployment | Vercel (static site hosting) |

---

## User Journey  
---

| Step | Screen |
|------|--------|
| Landing | `index.html` |
| Login | `signin.html` (auto-filled credentials) |
| Chat Dashboard | `chat.html` or main chat interface |
| Profile / Sidebar | Demo card elements for future expansion |

---

## Project Structure (Simplified)  
---
FloatChat/
├── index.html               # Landing page  
├── signin.html              # Login page (auto-filled credentials)  
├── chat.html                # Main chat UI  
├── assets/
│   ├── css/
│   │   └── style.css        # Core styles  
│   └── js/
│       └── script.js        # UI interactivity  
└── README.md

---

## Deployed Link  
---

**Live Demo:** [https://fluentme.vercel.app/](https://fluentme.vercel.app/)  
*(Open in Chrome/Edge for best experience)*

---

## Future Roadmap  
---

- Multi-user real-time chat via WebSocket/Firebase  
- Authentication system with JWT or OAuth  
- Message persistence and database integration  
- AI chatbot mode (using OpenAI API)  
- Dark mode toggle  

---

## Author  
---

**Hargun**  
Frontend & AI Enthusiast  

GitHub → @hargun144

