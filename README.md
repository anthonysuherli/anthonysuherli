## Anthony Suherli

Hi — I'm an ML engineer / researcher. My day job is on Vanguard's AI Garage team, where
I work on production ML and multi-agent systems for investment management. Over the last
few years that's meant moving from fairly classical ML pipelines toward agentic setups
and, more recently, knowledge systems that a lot of people end up depending on. I came
into all of this from a financial-engineering and electrical-engineering background, with
a few IEEE papers from earlier research days.

Outside of work I've been spending most of my time on **context engineering** — basically,
the question of how you feed an agent the right context so it reasons about something
instead of guessing. It turns out that's most of the work, and it's where the interesting
problems are: how you collect information, decide what's worth keeping, structure it, and
keep it from going stale. The projects below are all me poking at different corners of that.
(They also mostly share a number — *delapan* is Indonesian for eight, and the rest just
kept the theme.)

### Things I'm tinkering with

- **[delapan](https://github.com/anthonysuherli/delapan)** — the engine the others are
  built on. You point it at a topic, it goes off and researches (plan → search → crawl →
  extract → merge), and saves what it finds as structured notes you can reuse later instead
  of re-deriving from scratch. Runs entirely on your machine (SQLite + sqlite-vec) and talks
  over MCP, so tools like Claude Code can just use it.

- **[br8n](https://github.com/anthonysuherli/br8n)** — a small experiment in not losing your
  train of thought. When you get interrupted, it jots down what you were actually doing (the
  one-line "I think the bug is X" hypothesis, not just which files were open) and hands it
  back as a quick resume card when you return. It's a fork of delapan, repurposed for
  capturing developer context.

- **[person8](https://github.com/anthonysuherli/person8)** — a hackathon project (Google
  Cloud Rapid Agent). An agent that tries to actually finish a task rather than just chat:
  it plans, searches over Elastic, and comes back with a cited answer plus a sensible next
  step.

- **[hunter8](https://github.com/anthonysuherli/hunter8)** — a much more down-to-earth one.
  A Playwright script that fills out job applications from a spreadsheet and stops to let me
  handle anything open-ended. Mostly built because applying to jobs by hand is tedious.

### Background, roughly

- ML engineer / researcher at **Vanguard (AI Garage)** since 2021.
- **M.S. Financial Engineering**, USC · **B.S. Electrical Engineering**, University of Washington.
- Mostly live in Python these days; also TypeScript, SQL, R, MATLAB. Comfortable across the
  usual AWS ML stack and the agent/MCP tooling.

Always happy to chat about agents, context, or anything in that neighborhood —
[LinkedIn](https://linkedin.com/in/suherli) · anthonysuherli@gmail.com
