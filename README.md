# FluentMe  
---

**FluentMe** is a browser-based AI speech coaching platform designed to help users with stuttering or fluency issues practice speaking in a gamified way — with real-time speech feedback, fluency scoring, and a friendly UI.

Built originally for hackathon pitching — FluentMe demonstrates that real-time speech analysis + gamified learning can make speech therapy accessible, stigma-free & fun.

---

## Why FluentMe?  
---

Most speech improvement tools are boring or medical-feeling.  
**FluentMe** makes it game-like:

- **Multiple practice modes** — Read Aloud, Tongue Twisters, Numbers, etc.  
- **Instant feedback** as you speak  
- **Analytical scoring** — WPM, pauses, disfluencies, repetition events, etc.  
- **Session-by-session progress** screen  
- **Demo leaderboard** between peers (for motivation)  

---

## 🌟 Key Features  
---

| Feature | Description |
|----------|-------------|
| **Practice Modules** | 6 modes like Read Aloud, Words, Tongue Twisters, Answer Questions etc |
| **Real-Time Speech Capture** | Web Speech API + MediaRecorder + custom heuristics |
| **VAD (Voice Activity Detection)** | RMS-based detection to compute speaking time & pauses |
| **Fluency Analytics** | WPM, pause count, stutter-like event detection, WER etc |
| **Gamified UI** | Skill badges, streak visuals, motivational dashboard |
| **Leaderboard UI** | Static leaderboard card (demo for future real backend) |

---

## 🧠 Speech Processing Logic (High-Level)  
---

When the user speaks →  

1. Browser microphone is captured  
2. RMS-based VAD runs to detect silence vs voice frames  
3. Web Speech API is used to transcribe text  
4. Heuristics detect disfluency events (repetitions, prefix repeats, etc.)  
5. Metrics like WPM, duration, pauses, WER, etc., are extracted  
6. `localStorage` stores per-skill score (simple scoring system)  
7. Dashboard + profile pages visualize improvement  

All this runs purely on the **front-end** — no server required.  

---

## 🧩 Tech Stack  
---

| Layer | Technology |
|--------|-------------|
| **Core** | HTML, CSS, JavaScript |
| **Speech Recognition** | Web Speech API |
| **Audio Capture / VAD** | MediaRecorder, WebAudio API |
| **Charting / Stats** | Chart.js |
| **Storage** | localStorage (browser) |
| **UI Styling** | Tailwind CSS + custom CSS |

---

## 🔄 User Journey  
---

| Step | Screen |
|------|--------|
| Landing | `index.html` |
| Login/Signup | `login.html` |
| Dashboard | `dashboard.html` |
| Choose Module | `as.html` + `assessment.html` |
| Actual Practice + Voice Analytics | `quizfinal.html` + `quizfinal.js` |
| View My Results | `profile_final.html` |

---
## Deployed Link  
---

**Live Demo:** [https://fluentme.vercel.app/](https://fluentme.vercel.app/)  
*(Open in Chrome/Edge for best experience)*

---

## Future Roadmap  
---

- Integrate a backend to save user profiles & scores
- Multiplayer leaderboard (actual real-time XP tracking)
- ML-based fluency scoring model (instead of heuristic)
- Add conversational AI mode (chat-style practice)

---

## Author  
---

**Hargun**  
GitHub → @hargun144


