<div align="center">

<img src="assets/hero.svg" alt="Adrian Ademovic — autonomous systems, LLM pipelines, risk-gated execution" width="100%"/>

<p>
  <a href="https://www.linkedin.com/in/adrian-ademovic-75ba6a268/"><img src="https://img.shields.io/badge/LinkedIn-connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://leetcode.com/u/Adrian08/"><img src="https://img.shields.io/badge/LeetCode-Adrian08-F2A93B?style=for-the-badge&logo=leetcode&logoColor=0A0C10" alt="LeetCode"/></a>
  <a href="https://latentdev.de"><img src="https://img.shields.io/badge/latentdev.de-website-11151B?style=for-the-badge&logoColor=white" alt="Website"/></a>
  <a href="mailto:ademovic0@web.de"><img src="https://img.shields.io/badge/Email-reach%20out-7D8896?style=for-the-badge&logo=maildotcom&logoColor=white" alt="Email"/></a>
</p>

</div>

---

## What I build

Systems that run without me watching them, and fail in a way I can predict.

That is one idea applied to different domains: an equity bot that will refuse its own strongest signal if the risk layer says no, a market scanner that resolves a malformed model response to *no trade* rather than a guess, a prompt toolchain that ships the evaluation harness alongside the prompt because a prompt nobody measured is a prompt nobody trusts.

**Direction.** I am heading toward autonomy and defense technology — systems that have to act on their own, under uncertainty, and be wrong safely. The work below is deliberate practice for that: hard gates, fail-closed defaults, no-lookahead validation. I am not there yet, and I do not pretend the domain experience exists. The engineering discipline does.

---

## Selected work

| | Project | What it does |
|---|---|---|
| 🛰️ | **[stockpilot](https://github.com/AdrianAdem/stockpilot)** | Autonomous equity trading agent for Alpaca. Four weighted signal sources — momentum, mean reversion, 13F institutional filings and a two-tier Claude analyst — feed a hard risk gate: ATR trailing stops as real GTC broker orders, sector caps, drawdown circuit breakers. A strong signal can still be rejected; that is the design.<br/><sub>`Python` · `asyncio` · `FastAPI` · `Alpaca` · `Claude API` · no-lookahead backtesting</sub> |
| 📡 | **[polyedge](https://github.com/AdrianAdem/polyedge)** | Event-driven signal scanner for Polymarket. A cheap Haiku pass filters ~1,700 open markets before Sonnet analyses the survivors against news, macro and crypto flow — the tiering is what holds the run cost to a few dollars a day instead of hundreds. Quarter-Kelly sizing, paper-only execution.<br/><sub>`Python` · `asyncio` · `websockets` · `SQLite` · `Claude API` · `ruff` + CI</sub> |
| 🧩 | **[prompt-engineer-skill](https://github.com/AdrianAdem/prompt-engineer-skill)** | An Agent Skill that treats prompt engineering as a procedure, not a document: it routes to the right artifact first (hook, skill, subagent or prompt), sizes an eval set to the actual volume, and ships a linter and a benchmark so the result can be measured.<br/><sub>`Python` · `Claude Code` · agent skills · evals</sub> |
| 📊 | **[athlete-dashboard](https://github.com/AdrianAdem/athlete-dashboard)** | Self-hosted training and health tracker that unifies what vendors keep apart: strength logs with 1RM analytics, Strava cardio, barcode nutrition and daily Garmin biometrics in one Postgres schema — so "did my HRV drop when volume spiked?" is finally a query. <a href="https://adrianadem.github.io/athlete-dashboard/">Live demo →</a><br/><sub>`TypeScript` · `React 19` · `Supabase` · `Vite` · `Tailwind`</sub> |

All MIT-licensed, each with architecture notes and setup in its README.

---

## Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=py,ts,js,react,nextjs,fastapi,supabase,postgres,tailwind,git,docker,swift&theme=dark" alt="Python, TypeScript, JavaScript, React, Next.js, FastAPI, Supabase, Postgres, Tailwind, Git, Docker, Swift"/>

</div>

Day to day: **Python** (async, FastAPI, pandas) and **TypeScript** (React, Supabase). LLM pipelines with the **Claude API** — as a tool and as a product layer. **Swift/SwiftUI** currently in the learning phase.

---

## Also

- Computer Science @ **TU Darmstadt**, starting October 2026. Long-term: ML/AI.
- Running **[Latent](https://latentdev.de)** — web design and AI automation for local businesses around Frankfurt.
- Solving algorithm problems in Python and Java — arrays, strings, trees, DP.
- Karate and Judo, which is where the discipline for the rest of it came from.

<div align="center">
<img src="https://leetcard.jacoblin.cool/Adrian08?theme=dark&font=JetBrains%20Mono&ext=activity" alt="LeetCode statistics" width="500"/>
</div>

---

<div align="center">
<sub>Open to internships, working-student roles and collaboration — especially anything autonomous, safety-critical, or both.</sub>
</div>
