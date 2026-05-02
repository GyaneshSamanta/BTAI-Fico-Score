# BTAI — FICO Score & SECI Knowledge Cycle Simulators

**Two browser-based teaching simulators built for Business Technology & AI coursework: an expert-system FICO scorer, and an interactive walkthrough of Nonaka's SECI knowledge-creation model.**

![HTML5](https://img.shields.io/badge/HTML5-orange)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-38B2AC)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-yellow)

## About

- **What:** A repository of two self-contained, single-page web simulations. The first reproduces FICO credit-score logic for sample applicants; the second steps a user through the four phases of the SECI knowledge-creation spiral.
- **Who:** Group project by **Gyanesh Samanta** with teammates **Astha**, **Atish**, and **Stanya**.
- **When:** First commit 2025-07-17, last update 2026-02-01.
- **Where:** Built for the **BTAI (Business Technology & AI) club** as a coursework / educational deliverable.
- **Why:** Both FICO scoring and the SECI knowledge cycle are easier to learn by watching the rules fire on real inputs than by reading a textbook chapter — so we wrapped each as an interactive sandbox.

## The Story

### FICO Score Simulator

The FICO simulator is structured as a small **expert system**: it takes financial inputs (payment history, credit utilization, length of history, credit mix, new credit) and walks through the canonical FICO weighting to land on a final score, breaking down which components helped or hurt. Three pre-loaded personas — **Priya**, **Rohan**, and **Sunita** — give a fast way to see how very different financial behaviours land on the 300-850 scale, and a dark/light toggle keeps it readable in any lighting.

### SECI Knowledge Cycle Simulator

The SECI tool models Ikujiro Nonaka's organizational knowledge-creation spiral — **Socialization → Externalization → Combination → Internalization** — as a four-stage interactive flow. Users sit through a discussion log to capture tacit knowledge (Socialization), draft a document from it (Externalization), see it merged into a persistent knowledge base (Combination), and then re-apply it (Internalization). Each pass updates the knowledge base, so the loop tangibly *grows* something across iterations rather than just describing the theory.

Both apps are zero-dependency single HTML files — no build step, no backend, just open and run.

---

## Tech Stack

- **Markup / Style:** HTML5, CSS3, **Tailwind CSS** (via CDN)
- **Logic:** Vanilla JavaScript (ES6+)
- **Typography:** Google Fonts (Inter)
- **Hosting:** Any static file server / browser

## Repo Structure

```
BTAI-Fico-Score/
├── simulations/
│   ├── fico-score-simulator/
│   │   └── index.html        # expert-system FICO scorer
│   └── seci-knowledge-cycle/
│       └── index.html        # SECI 4-phase walkthrough
└── README.md
```

## Getting Started

No build tools, no install — just open the HTML files.

```bash
# 1. Clone
git clone https://github.com/GyaneshSamanta/BTAI-Fico-Score.git
cd BTAI-Fico-Score

# 2. Open whichever simulator you want
#    macOS / Linux
open simulations/fico-score-simulator/index.html
open simulations/seci-knowledge-cycle/index.html

#    Windows
start simulations/fico-score-simulator/index.html
```

Or serve the folder over a tiny local server if your browser blocks file:// fetches:

```bash
python -m http.server 8000
# then visit http://localhost:8000/simulations/
```

## Contributing

This is a coursework deliverable, but PRs that fix bugs, add personas, or extend the SECI knowledge base are welcome.

## License

Released for research and educational purposes. No formal OSS license has been published yet — please ask before commercial reuse.

## Credits

Made with care by:

- **Astha**
- **Atish**
- **Gyanesh Samanta** ([@GyaneshSamanta](https://github.com/GyaneshSamanta))
- **Stanya**

Built for the BTAI initiative.
