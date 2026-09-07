<img src="assets/hero.svg" alt="Adrian Ademovic — systems that act on their own, and are wrong safely" width="100%"/>

I build software that runs while nobody is watching it, and I care most about what it does when it is wrong. A trading agent whose risk layer is allowed to veto its own strongest signal. A market scanner that answers a malformed model response with *no signal* instead of a guess. A prompt toolchain that ships the evaluation harness next to the prompt, because a prompt nobody measured is a prompt nobody trusts.

I am heading toward defense technology and autonomy. I have no domain experience there yet and will not pretend otherwise — what I bring is the habit the domain runs on: hard gates, fail-closed defaults, no-lookahead validation, and no model output trusted without a check behind it.


<br>

---

<br>

### Systems

<table>
<tr><td width="180"><b><a href="https://github.com/AdrianAdem/stockpilot">stockpilot</a></b><br><sub>Python · Alpaca</sub></td>
<td>Autonomous equity agent. Momentum, mean reversion, 13F institutional flow and a two-tier Claude analyst weighted into one score.<br><sub><b>The constraint:</b> 0.25% of equity at risk per trade, sector caps, drawdown breakers. Stops rest at the broker as real GTC orders and fire while the bot is offline.</sub></td></tr>

<tr><td><b><a href="https://github.com/AdrianAdem/polyedge">polyedge</a></b><br><sub>Python · Polymarket</sub></td>
<td>Event-driven scanner for prediction markets. A cheap pass reads roughly 1,700 open markets; only survivors reach the expensive one.<br><sub><b>The constraint:</b> every call logs tokens, latency and USD. The tiering is the entire cost design, and a broken model response resolves to no signal.</sub></td></tr>

<tr><td><b><a href="https://github.com/AdrianAdem/prompt-engineer-skill">prompt-engineer</a></b><br><sub>Agent skill · Claude Code</sub></td>
<td>Turns a request into a prompt together with the tests that say whether it works.<br><sub><b>The constraint:</b> it decides the artifact first — hook, skill, subagent or prompt — because placement is what determines whether an instruction takes effect at all. Ships a linter and a benchmark, and passes its own linter.</sub></td></tr>

<tr><td><b><a href="https://github.com/AdrianAdem/athlete-dashboard">athlete-dashboard</a></b><br><sub>TypeScript · Supabase</sub></td>
<td>Self-hosted training and health tracker: strength logging, Strava cardio, barcode nutrition and daily Garmin biometrics.<br><sub><b>The constraint:</b> one Postgres schema behind row-level security, so "did my HRV drop in the weeks my volume spiked" is a query rather than four apps.</sub></td></tr>
</table>

<sub>All MIT. Architecture notes and setup live in each repository.</sub>


<br>

---

<br>

### How I work

**I write down what the system is not allowed to do before I write what it does.** Position caps, drawdown breakers and per-scan call budgets exist in these projects because an autonomous process without a ceiling is a process waiting to find one.

**Failure resolves to inaction, never to a guess.** Malformed model output, a missing feed, an API error: all of them end in "no trade", not in a default. Live execution in both trading projects is a deliberate stub that raises rather than a flag someone can flip by accident.

**A number I did not measure does not go in the README.** Backtests fill on the next open and check stops against intraday lows, because a result that quietly reads tomorrow's price is worse than no result.

<details>
<summary>What I am still learning</summary>

<br>

Swift and SwiftUI, currently at the level where I can build a screen but not yet architect an app. Deep CS fundamentals, which is what the degree is for. I do not have production DevOps experience beyond straightforward deploys, and I would rather say so than discover it in the first week.

</details>


<br>

---

<br>

### Stack

<div align="center">

<br>

<img src="https://skillicons.dev/icons?i=py,ts,js,react,nextjs,fastapi,supabase,postgres,tailwind,docker,git,github,vscode,swift&theme=dark&perline=7" alt="Python, TypeScript, JavaScript, React, Next.js, FastAPI, Supabase, Postgres, Tailwind, Docker, Git, GitHub, VS Code, Swift"/>

<br>


</div>

**Python** — asyncio, FastAPI, pandas, pytest, ruff &nbsp;·&nbsp; **TypeScript** — React, Supabase, Vite, Tailwind &nbsp;·&nbsp; **LLM pipelines** — Claude API, tiered routing, prompt caching, cost accounting. **Swift and SwiftUI** are in the learning phase, and I would rather say so than list them as a skill.


<br>

---

<br>

### Algorithms

<div align="center">

<img src="https://leetcard.jacoblin.cool/Adrian08?theme=dark&font=JetBrains%20Mono" alt="LeetCode statistics" width="520"/>

</div>


<br>

---

<br>

### Elsewhere

Computer Science at TU Darmstadt from October 2026. I run [**Latent**](https://latentdev.de) alongside it — web design and AI automation for owner-run businesses around Frankfurt, which is where I learned to ship something a stranger has to use on the first try. Karate and Judo.

<div align="center">

<a href="https://www.linkedin.com/in/adrian-ademovic-75ba6a268/"><img src="https://img.shields.io/badge/LinkedIn-connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0D1117" alt="LinkedIn"/></a> <a href="https://leetcode.com/u/Adrian08/"><img src="https://img.shields.io/badge/LeetCode-Adrian08-F0A032?style=for-the-badge&logo=leetcode&logoColor=white&labelColor=0D1117" alt="LeetCode"/></a> <a href="https://latentdev.de"><img src="https://img.shields.io/badge/Latent-latentdev.de-4C8DAE?style=for-the-badge&logo=safari&logoColor=white&labelColor=0D1117" alt="Website"/></a> <a href="mailto:ademovic0@web.de"><img src="https://img.shields.io/badge/Email-get%20in%20touch-D14836?style=for-the-badge&logo=maildotcom&logoColor=white&labelColor=0D1117" alt="Email"/></a>

<br>

</div>
