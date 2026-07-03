🚀 Agentic AI App Builder

Turn natural language into production-ready full-stack applications — instantly.
AI doesn’t just generate code — it plans, writes, improves, and debugs entire apps autonomously.

Built with Next.js + Gemini AI + Supabase + Agentic tooling, inspired by platforms like Bolt.new and Lovable.

⚡ What this is

Type a prompt like:

“Build a SaaS dashboard with auth, pricing, and analytics”

And the system will:

🧠 Generate full-stack React/Next.js code
🗂️ Create structured project files automatically
⚡ Run instantly in a live browser sandbox
🔧 Fix runtime errors using AI
🤖 Improve code using autonomous agents (Pro feature)
🎯 Why this project is different

Most AI tools just generate code.

This system:

Thinks in projects, not snippets
Maintains persistent workspace memory
Uses an AI agent loop (generate → run → fix → improve)
Supports real-time execution inside the browser
✨ Core Features
🧠 AI Code Generation Engine
Powered by Google Gemini (Flash model)
Structured output: files, dependencies, and metadata
Streaming responses with live progress updates
npm validation to prevent hallucinated packages
🤖 Agent Mode (Autonomous AI)
Built using Cline SDK
Can:
Modify files one-by-one
Refactor entire codebases
Stream reasoning in real-time
Uses tool-based execution:
update_file
done_improving
💬 Persistent AI Workspace
Chat history saved per project
Context-aware conversations
Resume any app generation anytime
🖥️ Live Code Sandbox (Sandpack)
Instant React app preview in browser
File explorer + code editor
Hot updates without full reload
Tailwind styling support
🧾 AI Debugging System
Detects runtime + compile errors
Auto “Fix with AI” button
Sends error context back to Gemini
Regenerates corrected code instantly
📦 Credit System
Plan	Credits
Free	10
Starter	50
Pro	150
1 credit = 1 generation or improvement
Protected on both client + server
Plan upgrades are additive (no loss of credits)
🧱 Tech Stack
Layer	Technology
Frontend	Next.js 15 (App Router, TypeScript)
Auth	Clerk
Database	Supabase (PostgreSQL)
ORM	Prisma
AI Engine	Google Gemini (Flash)
Agent System	Cline SDK
Preview Engine	Sandpack
UI	Tailwind CSS v4 + Shadcn UI
Rate Limiting	Arcjet
Storage	Supabase Storage
🏗️ System Architecture
🔷 High-Level Flow
User Prompt
   ↓
Next.js Chat UI
   ↓
API Layer (/api/gen-ai-code)
   ↓
Gemini AI (Code Generation Engine)
   ↓
Structured Output (Files + Dependencies)
   ↓
Supabase Database (Workspace Storage)
   ↓
Sandpack Sandbox (Live Preview)
   ↓
User sees running application ⚡
🤖 Agent Improvement Flow
User clicks “Improve with AI”
   ↓
Cline Agent starts execution
   ↓
Reads full project structure
   ↓
Updates files step-by-step
   ↓
Streams changes via SSE
   ↓
Sandpack auto-refreshes preview
   ↓
Optimized production-ready app 🚀
🧩 Architecture Diagram
🧑‍💻 Workspace System

Each workspace contains:

Chat messages (AI + user)
Generated file system
Dependency graph
Project metadata

Everything is persisted in Supabase.

🔐 Authentication & Billing
Google OAuth via Clerk
Automatic user sync to Supabase
Plan-based access control
Credit deduction per AI operation
Secure server + client validation
🗃️ Database Schema
User
id
clerkId
name
email
imageUrl
credits
plan
createdAt
updatedAt
Workspace
id
userId
title
messages (JSON)
fileData (JSON)
createdAt
updatedAt
⚙️ Getting Started
1. Clone repo
git clone https://github.com/your-repo/agentic-ai-app-builder
cd agentic-ai-app-builder
npm install
2. Setup database
npx prisma generate
npx prisma db push
3. Run development server
npm run dev
🔐 Environment Variables
# Clerk
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

# Supabase
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=
DATABASE_URL=

# Gemini AI
GEMINI_API_KEY=

# Arcjet
ARCJET_KEY=
🚀 What makes this project impressive
Real agentic AI system (not just prompt-response)
Full-stack SaaS architecture
Live execution sandbox (rare in AI tools)
Persistent AI memory per workspace
Multi-layer AI pipeline (generate → run → fix → improve)
Production-ready billing + auth system
🔮 Future Enhancements
Multi-agent collaboration system
GitHub repo export
One-click deployment to Vercel
Plugin ecosystem for tools
Real-time multiplayer AI coding
⭐ Show Your Support

If this project helped you learn AI systems or full-stack architecture:

⭐ Star the repo
🚀 Share with developers
🔥 Build something insane with it

🧠 Final Thought

This isn’t just an AI code generator.

It’s a self-improving software creation system powered by agents.