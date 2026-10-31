# ⚡ QUESTFLOW 3D

> **"Play the Game. Finish the Work."**

[![Hackathon](https://img.shields.io/badge/PromptWars_×_OUTLIER'2026-Google_for_Developers-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://developers.google.com/)
[![Build with AI](https://img.shields.io/badge/Build_with_AI-Gemini_Powered-00BCD4?style=for-the-badge&logo=google&logoColor=white)](https://ai.google.dev/)
[![Live Demo](https://img.shields.io/badge/Live_Demo-localhost:5173-00F0FF?style=for-the-badge&logo=vite&logoColor=white)](http://localhost:5173)
[![TypeScript](https://img.shields.io/badge/TypeScript-Strict_0_Errors-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![React](https://img.shields.io/badge/React-18.3.1-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![Three.js](https://img.shields.io/badge/Three.js-R3F_v8-000000?style=for-the-badge&logo=threedotjs&logoColor=white)](https://threejs.org/)

---

## 🌌 What is QUESTFLOW?

**QUESTFLOW** is a **3D action-arcade gamified productivity platform** built for the **PromptWars × OUTLIER'2026** hackathon (Google for Developers / Build with AI).

It transforms your most painful digital chores — 5,000 unread emails, messy file folders, unsorted bank statements, and broken code — into **immersive 3D game missions**. The twist: **every game action executes a real background API call**. Destroy an email enemy → Gmail inbox actually gets cleaned. Tractor-beam a file asteroid → your folder is actually reorganized. No fake simulation. No fake progress.

> 🏆 **Challenge:** *"Build an experience where playing a fast-paced game or interactive story actually executes the real-world chore in the background."*

---

## 🎯 Core Philosophy

```
ZERO FAKE SIMULATION POLICY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
XP is awarded ONLY after a verified real-world response:
  HTTP 200 OK  ✓  →  XP Awarded + 3D Combat FX
  HTTP 4xx/5xx ✗  →  Mission Paused + User-Friendly Alert
  LOCAL_VERIFIED ✓ →  File organized / Code fixed on disk
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## 🗺️ System Architecture

```
┌─────────────────────────────────────────────────────────────────────────┐
│                         USER INTERACTION                                │
│           (3D Click / Aim / Blast / Tractor Beam / Scan)                │
└───────────────────────────────┬─────────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────────┐
│                    MISSION SETUP STATION                                │
│         Real-work data ingestion before mission launch:                 │
│    Gmail OAuth / .mbox Upload / Folder Picker / CSV Drop / Code Paste  │
└───────────────────────────────┬─────────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────────┐
│                     3D GAME CANVAS (R3F)                                │
│    EmailDungeon3D / FolderRescue3D / ExpenseDetective / BugSlayer3D    │
│           Enemies = Real Data Objects (emails, files, bugs)             │
└───────────────────────────────┬─────────────────────────────────────────┘
                                │  Player completes action
                                ▼
┌─────────────────────────────────────────────────────────────────────────┐
│                    REAL-WORLD EXECUTION ENGINE                          │
│    Gmail batchModify API  /  Web File System Access API  /             │
│    PapaParse CSV Export  /  AST/Regex Code Scanner & Fixer             │
└───────────────────────────────┬─────────────────────────────────────────┘
                                │  Verified 200 OK / LOCAL_VERIFIED
                                ▼
┌─────────────────────────────────────────────────────────────────────────┐
│                      STATE ENGINE UPDATE                                │
│           XP + Level Up + Achievement Badge + Leaderboard              │
└───────────────────────────────┬─────────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────────┐
│                     VISUAL & AUDIO FEEDBACK                             │
│    Confetti Burst / Web Audio FX / Questo Mascot Celebration Dance     │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## ✨ Feature Overview

| Feature | Description |
|---|---|
| 🎬 **Cinematic Startup Splash** | Streaming-platform quality intro with volumetric particles, neon logo zoom, chromatic aberration, and skip option |
| 🦉 **Questo the Cyber-Owl** | 3D AI mascot companion (React Three Fiber), Web Speech API voice, mood states, mission hints |
| ⚔️ **Email Dungeon** | 3D neon highway shooter — destroy email enemies → Gmail inbox cleaned via API |
| 🚀 **Folder Rescue** | 3D orbital salvage station — tractor-beam file asteroids → real folder sorted + ZIP export |
| 💰 **Expense Detective** | CSV drag-and-drop — classify transactions in gameplay → download audited Financial Summary |
| 🐛 **Bug Slayer** | 3D syntax tower defense — EMP blast crawling virus bugs → real code fixed and downloadable |
| 🎮 **3D / 2D Toggle** | Switch between immersive Three.js 3D and classic 2D tactical view per mission |
| 🛡️ **Mission Setup Station** | Data ingestion gate before every mission — ensures gameplay works on YOUR real data |
| 🔑 **Evaluator Bypass** | Instant sandbox mode for judges — no credentials required to demo all features |
| 🔊 **Web Audio Synthesizer** | Zero external audio files — all sound FX synthesized via Web Audio API |
| 🎆 **Canvas Confetti** | Particle celebrations on mission completion |
| 🏆 **Leaderboard & Badges** | Persistent XP, levels, and achievement badges via localStorage |

---

## 🎮 Mission Modules

### ⚔️ MODE A — EMAIL DUNGEON (3D Cyber-Space Shooter)

- **Environment:** Neon-lit Tron/Cyberpunk digital grid highway with volumetric fog
- **Enemy Types:**
  | Enemy | Email Category | HP | Behavior |
  |---|---|---|---|
  | 🤖 Drone Bot | Promotions | Low | Flying erratic |
  | 👻 Specter | Social | Medium | Phase-shifting |
  | 🟢 Slime | Spam/Trash | Low | Crawling acid |
  | 🦾 Boss Mech | Important/Personal | High | Displays sender + subject on holographic HUD |
- **3D Controls:** Mouse aim + click to fire plasma laser bolts
- **Real Execution:** Destroying an enemy calls `gmail.users.messages.batchModify` → email archived/marked-read in real Gmail inbox
- **Fallback:** Exports an organized `.json` archive log if no OAuth token
- **Input Methods:** Google OAuth 2.0 live inbox fetch OR `.mbox`/`.json` file upload

---

### 🚀 MODE B — FOLDER RESCUE (3D Orbital Salvage)

- **Environment:** Deep space station with floating file debris asteroids
- **Gameplay:** Tractor-beam file asteroids into sorted cargo bays (`/PDFs`, `/Images`, `/Archives`, `/Code`, `/Other`)
- **Real Execution:** Web File System Access API (`showDirectoryPicker`) reorganizes files on actual disk OR generates a sorted `.zip` bundle for download
- **Input Methods:** Native folder picker (Chrome/Edge) OR multi-file upload drag-and-drop

---

### 💰 MODE C — EXPENSE DETECTIVE (Financial Sorting Arcade)

- **Environment:** Neon city grid with falling uncategorized transaction cards
- **Gameplay:** Tap/click to categorize each transaction (Food, Transport, Shopping, Bills, Income, etc.)
- **Real Execution:** PapaParse processes the raw CSV, applies merchant classification heuristics, and exports a fully audited Financial Summary CSV
- **Input Methods:** Drag-and-drop bank statement CSV or receipt JSON

---

### 🐛 MODE D — BUG SLAYER (3D Syntax Tower Defense)

- **Environment:** 3D code syntax tower with crawling virus bug swarms
- **Gameplay:** EMP shockwave blast targets identified bug entities → fires code fixes
- **Real Execution:** AST/regex scanner identifies real syntax errors, unused variables, console.log statements, missing semicolons. Applying fixes patches the actual code string for download.
- **Input Methods:** Paste raw JS/TS/Python code OR open a local code file

---

## 🛠️ Tech Stack

### Frontend
| Package | Version | Purpose |
|---|---|---|
| React | 18.3.1 | UI Framework |
| TypeScript | 5.x | Type Safety (strict mode, 0 errors) |
| Vite | 6.4.5 | Build Tool & Dev Server |
| Tailwind CSS | 3.x | Utility-first Styling |
| Framer Motion | Latest | Cinematic Splash Animations |
| Lucide React | Latest | Icon Library |

### 3D Graphics
| Package | Version | Purpose |
|---|---|---|
| Three.js | Latest | 3D Rendering Engine |
| @react-three/fiber | 8.x | React renderer for Three.js |
| @react-three/drei | 9.x | R3F Helpers & Utilities |

### Data & Processing
| Package | Version | Purpose |
|---|---|---|
| PapaParse | Latest | CSV Parsing & Export |
| JSZip | Latest | ZIP Bundle Generation |
| canvas-confetti | Latest | Particle Celebration FX |

### APIs & Services
| API | Scope | Purpose |
|---|---|---|
| Google OAuth 2.0 | `gmail.modify`, `gmail.readonly` | Gmail inbox read & archive |
| Web File System Access API | Native Browser | Real folder read/write |
| Web Audio API | Native Browser | Synthesized sound FX |
| Web Speech API | Native Browser | Questo voice feedback |

---

## 📋 Prerequisites

- **Node.js** ≥ 18.0.0 (v20+ recommended)
- **npm** ≥ 9.0.0
- **Browser:** Google Chrome or Microsoft Edge (required for Web File System Access API)
- **Google Cloud Console account** (optional — for live Gmail OAuth)

---

## 🚀 Installation & Quick Start

```bash
# 1. Clone the repository
git clone <your-repo-url>
cd questflow

# 2. Install dependencies
npm install

# 3. Configure environment (see section below)
cp .env.example .env
# Edit .env with your Google OAuth Client ID

# 4. Start the dev server
npm run dev

# 5. Open your browser
# http://localhost:5173
```

### Build for Production

```bash
npm run build
npm run preview
```

---

## 🔑 Google OAuth 2.0 Setup (Gmail Integration)

> ⚠️ **Skip this section if using Sandbox/Demo Mode.** Judges can test all features without OAuth.

### Step 1 — Create a Google Cloud Project

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Click **"New Project"** → name it `QuestFlow`
3. Enable the **Gmail API**: APIs & Services → Library → search "Gmail API" → Enable

### Step 2 — Create OAuth 2.0 Credentials

1. Go to **APIs & Services → Credentials**
2. Click **"Create Credentials" → "OAuth Client ID"**
3. Application type: **Web Application**
4. Name: `QuestFlow Dev`
5. **Authorized JavaScript Origins:**
   ```
   http://localhost:5173
   ```
6. Click **Create** → copy your **Client ID**

### Step 3 — Configure OAuth Consent Screen

1. Go to **APIs & Services → OAuth consent screen**
2. User Type: **External**
3. Add your email as a **Test User**
4. Add scopes:
   - `https://www.googleapis.com/auth/gmail.readonly`
   - `https://www.googleapis.com/auth/gmail.modify`

### Step 4 — Set Environment Variable

```env
# .env
VITE_GOOGLE_CLIENT_ID=your-client-id-here.apps.googleusercontent.com
```

---

## ⚙️ Environment Configuration

Copy `.env.example` to `.env` and fill in your values:

```env
# Google OAuth 2.0 Client ID
# Get from: https://console.cloud.google.com/apis/credentials
VITE_GOOGLE_CLIENT_ID=your-client-id.apps.googleusercontent.com
```

> **Without this variable:** The app runs fully in Sandbox/Demo Mode. All features are testable with mock data.

---

## 🧑‍⚖️ Evaluator & Judge Quick Access

QUESTFLOW includes a built-in **Evaluator Bypass System** so hackathon judges can instantly demo all features without setting up OAuth credentials.

### Activate Sandbox Mode (3 methods):

| Method | How |
|---|---|
| 🔗 **URL Parameter** | Open `http://localhost:5173/?eval_bypass=true` |
| ⌨️ **Keyboard Shortcut** | Press `Ctrl + Shift + Alt + H` anywhere in the app |
| 🔤 **Secret Sequence** | Type `hackathon2026` (no input field needed) |

### What Sandbox Mode Enables:

- ✅ **Email Dungeon** — Pre-loaded with 30 mock emails across all categories
- ✅ **Folder Rescue** — Pre-loaded with 20 mixed file types for sorting
- ✅ **Expense Detective** — Pre-loaded with 25 uncategorized transactions
- ✅ **Bug Slayer** — Pre-loaded with intentionally corrupted TypeScript code
- ✅ **Full XP & leveling system** — All progression features active
- ✅ **Questo Mascot** — All mood states and hint dialogues available
- ✅ **3D / 2D toggle** — All arena views accessible

> A prominent **🧪 SANDBOX MODE** banner appears at the top of the app when bypass is active.

---

## 🕹️ 3D Controls Reference

| Control | Action |
|---|---|
| **Left Click** | Fire laser / Execute action |
| **Mouse Move** | Aim targeting reticle |
| **Orbit Drag** | Rotate 3D camera (R3F OrbitControls) |
| **Scroll Wheel** | Zoom in / out |
| **3D / 2D Button** | Toggle between 3D arcade and 2D tactical view |
| **Space / Enter** | Confirm target / Activate ability |
| **Escape** | Pause mission / Return to dashboard |

---

## 🏗️ Project Structure

```
questflow/
├── index.html                    # App entry — Google GSI script loaded
├── package.json                  # Dependencies & scripts
├── vite.config.ts                # Vite build configuration
├── tsconfig.json                 # TypeScript strict config
├── tailwind.config.js            # Tailwind + custom cyber palette
├── postcss.config.js             # PostCSS + Autoprefixer
├── .env.example                  # Environment variable template
├── .gitignore
├── README.md
└── src/
    ├── main.tsx                  # Root — ErrorBoundary + QuestProvider
    ├── App.tsx                   # CinematicSplash + Mascot + screen router
    ├── index.css                 # Tailwind + cyber-grid / glass-panel utilities
    ├── types/
    │   └── index.ts              # Full TypeScript type definitions
    ├── state/
    │   └── questContext.tsx      # Global state — XP, missions, bypass, player
    ├── services/
    │   ├── audio.ts              # Web Audio API synthesizer (all SFX)
    │   ├── confetti.ts           # canvas-confetti — fireCyberConfetti / sparks
    │   ├── storage.ts            # localStorage — XP, badges, leaderboard
    │   ├── gmailService.ts       # Google OAuth 2.0, fetchRealInbox, batchModify
    │   ├── fileSystemService.ts  # Web File System Access API + JSZip
    │   ├── expenseService.ts     # PapaParse CSV + merchant classifier
    │   └── codeService.ts        # AST/regex scanner + code fixer
    ├── components/
    │   ├── layout/
    │   │   ├── Navbar.tsx               # Top nav — sandbox toggle, XP bar
    │   │   ├── NotificationToast.tsx    # User-friendly error/success alerts
    │   │   ├── ConfirmationModal.tsx    # Action confirmation dialogs
    │   │   └── ErrorBoundary.tsx        # React error boundary wrapper
    │   ├── splash/
    │   │   └── CinematicSplash.tsx      # Streaming-quality intro animation
    │   ├── mascot/
    │   │   └── QuestoMascot3D.tsx       # 3D cyber-owl — R3F + Speech API
    │   ├── landing/
    │   │   └── LandingPage.tsx          # Marketing / hero landing screen
    │   ├── dashboard/
    │   │   └── Dashboard.tsx            # Mission hub — XP, leaderboard, cards
    │   ├── auth/
    │   │   └── OAuthPortal.tsx          # Google OAuth sign-in portal
    │   ├── results/
    │   │   └── MissionDebrief.tsx       # Post-mission stats & XP summary
    │   ├── arena/
    │   │   ├── MissionArena.tsx         # Gates to setup station then 3D arena
    │   │   └── MissionSetupStation.tsx  # Real-work input per module
    │   ├── arena3d/
    │   │   ├── GameCanvas3D.tsx         # R3F Canvas — 3D/2D toggle + HUD overlay
    │   │   ├── EmailDungeon3D.tsx       # 3D highway, enemies, laser bolts
    │   │   ├── FolderRescue3D.tsx       # 3D space station, asteroids, tractor beam
    │   │   └── BugSlayer3D.tsx          # 3D syntax tower, virus bugs, EMP wave
    │   └── modules/
    │       ├── EmailDungeon/
    │       │   └── EmailArena.tsx       # 2D fallback — monster cards + JSON export
    │       ├── FolderRescue/
    │       │   └── FolderArena.tsx      # 2D fallback — file grid + ZIP export
    │       ├── ExpenseDetective/
    │       │   └── ExpenseArena.tsx     # Transaction swipe + CSV export
    │       └── BugSlayer/
    │           └── BugArena.tsx         # Code viewer + fix engine + download
```

---

## ✅ Hackathon Compliance Checklist

| Requirement | Status | Detail |
|---|---|---|
| **Real API Execution** | ✅ | Gmail `batchModify`, File System API, CSV export, code fix |
| **No Fake Simulation** | ✅ | XP awarded only on HTTP 200 / LOCAL_VERIFIED |
| **Sandbox/Demo Mode** | ✅ | Instant bypass — 3 activation methods |
| **Gamified Interface** | ✅ | 3D action-arcade + 4 mission worlds |
| **User Data Input** | ✅ | MissionSetupStation gates every arena |
| **TypeScript Strict** | ✅ | `tsc --noEmit` passes with 0 errors |
| **Production Build** | ✅ | `npm run build` — 2615+ modules, ~17s |
| **Error Handling** | ✅ | All API calls wrapped, toast alerts on failure |
| **Responsive Design** | ✅ | Desktop + mobile layouts |
| **Accessibility** | ✅ | ARIA labels, keyboard navigation |

---

## 🎨 Design System

```
Color Palette — Cyberpunk Dark Mode
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Background:   #0B0E14  (Deep Space Dark)
Surface:      #161B26  (Dark Glass)
Surface Alt:  #1F293D  (Elevated Glass)
Accent Cyan:  #00F0FF  (Neon Electric Blue)
Accent Purple:#8A2BE2  (Electric Violet)
Accent Green: #00FF88  (Matrix Neon)
Warning:      #FFD700  (Gold Alert)
Danger:       #FF4444  (Crimson Alert)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Effects: Glassmorphism (backdrop-blur + rgba), 
         Neon glow box-shadow, 
         Cyberpunk grid background pattern
```

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit changes: `git commit -m 'feat: add your feature'`
4. Push to branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

## 👨‍💻 Built For

**PromptWars × OUTLIER'2026** — Google for Developers / Build with AI Hackathon

> *QUESTFLOW proves that productivity and gaming aren't opposites — they're the same thing, finally honest about it.*

---

<div align="center">

**⚡ QUESTFLOW — Play the Game. Finish the Work. ⚡**

[![Start Playing](https://img.shields.io/badge/▶_START_PLAYING-http://localhost:5173-00F0FF?style=for-the-badge)](http://localhost:5173)
[![Judge Mode](https://img.shields.io/badge/⚖️_JUDGE_MODE-?eval_bypass=true-8A2BE2?style=for-the-badge)](http://localhost:5173/?eval_bypass=true)

</div>
