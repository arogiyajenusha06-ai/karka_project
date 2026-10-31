# KARKA NEXUS — INTELLIGENCE IN MOTION

> **"Where human curiosity meets artificial intelligence."**  
> **"Don't just use AI. Build what's next."**

**KARKA NEXUS** is a full-stack web platform built for **Karka AI & Tech Academy** (Nagercoil, Tamil Nadu). It combines an editorial futuristic design system, an interactive 3D Neural Intelligence Orb, an AI Prompt Engineering Lab, and **NEXA** — a personal AI guide powered by an Express/Node.js backend with live LLM integration and deterministic knowledge fallback.

---

## 🌟 Key Features

1. **Futuristic Visual Design System & Dual Theme**
   - **Dark Theme (`#070B1D`)**: Deep navy matrix with glowing cyan accents (`#25E6F7`) and electric blue hues (`#3578FF`).
   - **Light Theme (`#F5F8FF`)**: High-contrast, clean editorial layout with crisp readability and blue accents (`#087FCE`).
   - Smooth theme transition, auto-detection of OS preferences, and persistent localStorage sync.

2. **Hero Section with Interactive 3D Neural Intelligence Orb**
   - Canvas-rendered 3D particle sphere with mathematical perspective projection.
   - Interactive mouse-responsive parallax easing.
   - Layered orbital rings and floating telemetry badges: `GENERATIVE AI`, `AI AGENTS`, `LLMs`, `AUTOMATION`, `INNOVATION`.

3. **Interactive AI Prompt Lab ("YOUR IDEAS. OUR INTELLIGENCE.")**
   - Playground allowing visitors to input any raw concept and select from 5 objectives:
     - *Build an AI Application*
     - *Create Content*
     - *Automate a Workflow*
     - *Develop a Chatbot*
     - *Generate a Business Idea*
   - Generates an architected prompt with context grounding, JSON schema definitions, guardrails, and copy-to-clipboard functionality.

4. **Generative AI Mastery Flagship Course Section**
   - Verified metadata: **6 Months duration**, **48 Lessons**, **Blended mode** (offline at Nagercoil campus + online hybrid).
   - Expandable interactive syllabus modules:
     - **Module 1: Advanced LLMs** (Fine-tuning Techniques, PEFT/LoRA, Model Evaluation)
     - **Module 2: Custom AI Solutions** (Autonomous AI Agents, Function Calling, Multi-modal AI)
     - **Module 3: Enterprise AI** (Scaling AI Workloads, Data Privacy in GenAI, Cost Management)
   - 3-step admission process (Application → Technical Interview → Enrollment).
   - Direct link to [Official GenAI Mastery Syllabus](https://www.karka.academy/courses/genai-mastery).

5. **AI Career Learning Journey**
   - Serpentine connected roadmap spanning 7 progressive stages:
     1. Discover AI
     2. Understand Generative AI
     3. Master Prompt Engineering
     4. Explore Large Language Models
     5. Develop AI Applications
     6. Build Real-World Projects
     7. Prepare for Career Opportunities
   - Deep-dive panel with tools and competencies.

6. **Project Showcase & Architecture Blueprints**
   - Production blueprints: *AI Knowledge Assistant (RAG)*, *Intelligent Workflow Automation*, *Generative Content Studio*.
   - Deep-dive architecture modal with latency metrics, recall statistics, and system design details.

7. **Karka Ecosystem Platforms**
   - **Spike AI**: Custom AI-guided learning companion (`spike.karka.academy`).
   - **Karka Infini AI**: Inter-college technology tournament with ₹1,00,000 prize pool (`infini.karka.academy`).

8. **Career Acceleration & Pay After Placement**
   - Verified **Zero Upfront Fees (Pay After Placement)** terms.
   - Verified **95% placement rate** and hiring partners: *Amazon, TCS, HCL, Matrimony.com, Novac, Capecom, Flow, Sodisys*.
   - 1-on-1 industry mentoring, unlimited mock technical interviews, and guaranteed agency internship.

9. **NEXA — Personal AI Assistant**
   - Floating circular assistant button with glowing neural orb and breathing animation.
   - Expandable chat drawer with quick suggestion chips, conversation history retention, and markdown rendering.
   - Full-stack integration with `POST /api/chat`.
   - Dual-mode architecture: seamlessly connects to live **Google Gemini 1.5** when `GEMINI_API_KEY` is provided, or executes the high-precision **Karka Deterministic Knowledge Engine** with verified institutional facts when running in demo/offline mode.

---

## 🏗️ Architecture & Project Structure

```
karka-nexus/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.tsx           # Sticky nav with logo, links & theme toggle
│   │   │   ├── ThemeToggle.tsx      # Animated sun/moon switch
│   │   │   ├── Hero.tsx             # Editorial typography & stats
│   │   │   ├── NeuralOrb.tsx        # 3D Canvas particle sphere & orbital rings
│   │   │   ├── AboutSection.tsx     # Karka Academy story & 6 pillars
│   │   │   ├── CourseSection.tsx    # GenAI Mastery syllabus & admission steps
│   │   │   ├── PromptLab.tsx        # Interactive prompt transformation lab
│   │   │   ├── LearningJourney.tsx  # 7-stage connected timeline roadmap
│   │   │   ├── ProjectShowcase.tsx  # Interactive project blueprints & modal
│   │   │   ├── PlatformsSection.tsx # Spike AI & Infini competitions
│   │   │   ├── CareerSection.tsx    # Career flywheel & Pay After Placement
│   │   │   ├── FAQ.tsx              # Interactive accordion
│   │   │   ├── EnrollmentCTA.tsx    # Consultation inquiry form
│   │   │   ├── Footer.tsx           # Verified links, contacts & branding
│   │   │   └── NexaChatbot.tsx      # Floating assistant launcher & chat drawer
│   │   ├── context/
│   │   │   └── ThemeContext.tsx     # Dark/light theme state & persistence
│   │   ├── App.tsx                  # Main layout assembler
│   │   ├── main.tsx                 # Entry mount
│   │   └── index.css                # CSS variables, tokens & utilities
│   ├── index.html                   # Fonts (Space Grotesk, Inter) & SEO tags
│   ├── vite.config.ts               # Tailwind v4 plugin & /api proxy to backend
│   └── package.json
│
├── backend/
│   ├── src/
│   │   ├── config/
│   │   │   └── systemPrompt.ts      # NEXA system instructions & verified facts
│   │   ├── controllers/
│   │   │   └── chatController.ts    # Input validation & error handlers
│   │   ├── middleware/
│   │   │   └── rateLimiter.ts       # Express IP rate limiter (30 req/min)
│   │   ├── routes/
│   │   │   └── chat.ts              # /api/chat & /api/health routes
│   │   ├── services/
│   │   │   └── aiService.ts         # Gemini LLM caller & deterministic fallback
│   │   └── server.ts                # Express server with CORS & JSON parser
│   ├── .env.example
│   ├── .env
│   ├── tsconfig.json
│   └── package.json
│
├── package.json                     # Root orchestrator scripts
└── README.md
```

---

## 🚀 Getting Started

### 1. Prerequisites
- **Node.js** v20+ 
- **npm** v10+

### 2. Installation
Install dependencies for both frontend and backend:
```bash
# Frontend
cd frontend
npm install

# Backend
cd ../backend
npm install
```

### 3. Running Locally
Run the development servers:

**Option A: Run concurrently from root**
```bash
npm run dev:backend   # Starts backend on http://localhost:5000
npm run dev:frontend  # Starts frontend on http://localhost:5173
```

**Option B: Run from individual folders**
```bash
# Terminal 1: Backend API
cd backend
npm run dev

# Terminal 2: Frontend Client
cd frontend
npm run dev
```

Visit **`http://localhost:5173/`** in your browser.

---

## 🤖 Configuring Live AI with Google Gemini (Optional)

The NEXA assistant operates out-of-the-box using its built-in **Deterministic Knowledge Engine**. If you would like to enable live LLM generation:

1. Obtain a free API key from [Google AI Studio](https://aistudio.google.com/).
2. Open `backend/.env` and insert your key:
   ```env
   GEMINI_API_KEY=your_gemini_api_key_here
   ```
3. Restart the backend server. NEXA will automatically switch to **Live Gemini 1.5** mode.

---

## 🏛️ Verified Karka Academy Details

- **Official Website:** [https://www.karka.academy/](https://www.karka.academy/)
- **GenAI Course:** [https://www.karka.academy/courses/genai-mastery](https://www.karka.academy/courses/genai-mastery)
- **Official Instagram:** [@karka.ai](https://www.instagram.com/karka.ai/)
- **Campus Location:** Nagercoil, Kanyakumari District, Tamil Nadu 629001
- **Contact Desk:** +91 9487530243 | `contact@karka.academy`
