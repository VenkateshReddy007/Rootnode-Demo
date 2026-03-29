<p align="center">
  <img src="https://img.shields.io/badge/HACK'A'WAR-2026-06b6d4?style=for-the-badge&labelColor=020817" />
  <img src="https://img.shields.io/badge/PS_2.4-Automating_Ops_Workflows-7c3aed?style=for-the-badge&labelColor=020817" />
  <img src="https://img.shields.io/badge/Status-Live-10b981?style=for-the-badge&labelColor=020817" />
</p>

<h1 align="center">
  <br>
  🌐 RootNode
  <br>
  <sub>AI-Powered Cloud Migration Wave Planner</sub>
</h1>

<p align="center">
  <strong>Enterprise migrations take 18 months and cost $2M in consulting fees.</strong><br>
  RootNode analyzes your application portfolio, builds a dependency graph,<br>
  and generates an optimized wave plan — <strong>in 8 seconds.</strong>
</p>

<p align="center">
  <a href="#-the-problem">Problem</a> •
  <a href="#-how-it-works">How It Works</a> •
  <a href="#-tech-stack">Tech Stack</a> •
  <a href="#-features">Features</a> •
  <a href="#-architecture">Architecture</a> •
  <a href="#-the-team">Team</a>
</p>

---

## 🔥 The Problem

Cloud migrations are a **$500B industry** riddled with failure:

| Metric | Reality |
|--------|---------|
| 💰 **$2M+** | Average consulting cost for migration planning |
| ⏱️ **18 months** | Typical planning timeline |
| 📉 **38%** | Migrations that fail or overspend |
| 📊 **500+** | App dependencies manually tracked in spreadsheets |

> **"Companies pay consultants $2M to produce spreadsheets. We do it in 8 seconds with AI."**

---

## ⚡ How It Works

RootNode replaces months of consulting with an **8-step AI pipeline** that runs in seconds:

```
📤 Upload Portfolio → 🔗 Build DAG → 📊 Generate Waves → ⚠️ Score Risk
      ↓                                                        ↓
🤖 AI Explanation ← 📦 Final Output ← ⏱️ Estimate Timeline ← 🔄 Assign Strategy
```

| Step | What Happens |
|------|-------------|
| **1. Build DAG** | Parse portfolio → networkx directed acyclic graph |
| **2. Generate Waves** | Topological sort respecting all dependency constraints |
| **3. Optimize** | Balance business priority + risk across waves |
| **4. Score Risk** | 4-factor scoring: criticality, data size, deps, complexity |
| **5. Assign Strategy** | Rehost / Replatform / Refactor (3R model) |
| **6. Estimate Timeline** | Complexity-based duration per app |
| **7. Structured Output** | Full JSON with waves, risks, strategies, timelines |
| **8. AI Explanation** | Amazon Bedrock explains every decision in plain English |

---

## 🛠️ Tech Stack

<table>
<tr>
<td align="center"><strong>Frontend</strong></td>
<td>React · React Flow · Recharts · Framer Motion · Glassmorphism CSS</td>
</tr>
<tr>
<td align="center"><strong>Backend</strong></td>
<td>Python 3.11 · AWS Lambda · networkx</td>
</tr>
<tr>
<td align="center"><strong>AI/ML</strong></td>
<td>Amazon Bedrock · Claude Sonnet · Prompt Engineering</td>
</tr>
<tr>
<td align="center"><strong>Cloud</strong></td>
<td>API Gateway · Amazon S3 · DynamoDB · IAM</td>
</tr>
<tr>
<td align="center"><strong>Deploy</strong></td>
<td>Vercel (Frontend) · AWS Lambda (Backend)</td>
</tr>
</table>

---

## ✨ Features

### 🎯 Core Engine
- **Dependency DAG Analysis** — Automatically maps all application relationships
- **Wave Planning** — Generates 3-5 migration waves respecting every dependency
- **Risk Scoring** — 4-factor composite risk for each application
- **Strategy Assignment** — Rehost / Replatform / Refactor per app
- **AI Explanations** — Amazon Bedrock explains WHY each decision was made

### 📊 Visualizations
- **Interactive Dependency Graph** — Draggable nodes, color-coded by wave
- **Gantt Timeline** — Visual wave timeline with strategy & risk overlay
- **Risk Heatmap** — Apps × risk factors matrix with color-coded cells
- **Cost Breakdown** — Donut + bar charts for strategy distribution & wave duration

### 🎨 Design
- **Futuristic Glassmorphism** — Deep space theme with glass cards and glow effects
- **Animated Mesh Background** — Floating gradient orbs with CSS keyframes
- **Micro-Animations** — Hover glows, scroll counters, staggered reveals
- **Oversized Typography** — Syne + Inter from Google Fonts
- **Fully Responsive** — Mobile, tablet, and desktop optimized

### 🔄 Interactive Demo
- Pre-filled portfolio data in a code-editor style textarea
- Click → 2s loading animation with status cycling
- Wave plan output with risk badges, strategy tags, and AI insights
- Three switchable visualization tabs (Graph / Gantt / Heatmap)

---

## 🏗️ Architecture

```
┌──────────────┐     CSV/JSON     ┌──────────────┐     invoke     ┌──────────────┐
│    React     │ ──────────────→  │ API Gateway  │ ────────────→  │  AWS Lambda  │
│   Frontend   │                  │   (REST)     │                │  (Python)    │
└──────────────┘                  └──────────────┘                └──────┬───────┘
                                                                        │
                                                            ┌───────────┼───────────┐
                                                            ▼           ▼           ▼
                                                    ┌──────────┐ ┌──────────┐ ┌──────────┐
                                                    │ Bedrock  │ │    S3    │ │ DynamoDB │
                                                    │ (Claude) │ │ (Plans) │ │(History) │
                                                    └──────────┘ └──────────┘ └──────────┘
```

---

## 📋 PS 2.4 Compliance

| Requirement | Status |
|-------------|--------|
| Ingests application portfolio with dependencies | ✅ |
| Maps dependencies using DAG | ✅ |
| Generates 3–5 wave plan respecting dependencies | ✅ |
| Highlights high-risk applications | ✅ |
| Visual dependency graphs & timeline estimates | ✅ Bonus |
| Migration strategy assignment (3R) | ⭐ Beyond spec |
| "What-if" live refinement | ⭐ Beyond spec |

---

## 🏆 What Makes This Different

```diff
+  ✓ DAG-based dependency analysis (not just lists)
+  ✓ Topological sort guarantees valid wave ordering
+  ✓ 4-factor risk scoring with weighted composites
+  ✓ AI explains every decision — not a black box
+  ✓ Three interactive visualizations, not static charts
+  ✓ 8 seconds vs 18 months of consulting

-  ✗ Manual consultants: $2M, 18 months, spreadsheets
-  ✗ AWS Migration Hub: No wave planning, no AI
-  ✗ Generic AI: Hallucinated plans with no graph analysis
```

---

## 🚀 Quick Start

```bash
# Clone the repo
git clone https://github.com/VenkateshReddy007/Rootnode-Demo.git

# Open locally — no build step needed
open index.html

# Or deploy to Vercel
vercel --prod
```

---

## 📁 Project Structure

```
Rootnode-Demo/
├── index.html        # Landing page — hero, demo, visualizations
├── solution.html     # Technical deep dive — engine, code, charts
├── styles.css        # Shared glassmorphism design system
├── vercel.json       # Vercel deployment configuration
└── README.md
```

---

## 👥 The Team

<table>
<tr>
<td align="center"><strong>Venkatesh Reddy K</strong><br><sub>Backend Lead / AWS Infra</sub><br><code>Python · Lambda · S3 · DynamoDB</code></td>
<td align="center"><strong>Akash Biswas</strong><br><sub>AI/ML Lead</sub><br><code>Bedrock · Claude · networkx</code></td>
<td align="center"><strong>HM Pranav</strong><br><sub>Frontend Lead</sub><br><code>React · Recharts · React Flow</code></td>
<td align="center"><strong>Babar Bashir Dar</strong><br><sub>Demo + Design</sub><br><code>UI/UX · SVG · Animation</code></td>
</tr>
</table>

---

<p align="center">
  <strong>Built with ☕ at RIT Bengaluru · HACK'A'WAR 2026</strong>
  <br><br>
  <img src="https://img.shields.io/badge/RootNode-Plan_built._Migration_starts.-06b6d4?style=for-the-badge&labelColor=020817" />
</p>
