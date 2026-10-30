# Hi, I'm Bartosz

Senior QA engineer. I design end-to-end test suites and the test infrastructure behind them, for web, mobile and APIs, in e-commerce, healthcare and SaaS.

## Test engineering

**[e2e-casebook](https://github.com/bartech-lab/e2e-casebook)** · [live demo](https://e2e-proving-ground.onrender.com)

A web app I built to be hard to test: [202 cases](https://github.com/bartech-lab/e2e-casebook/tree/main/cases) such as realtime chat with reconnects, offline queues, time zones and DST, payments in frames and accessibility.

- The server exposes [72 documented test hooks](https://github.com/bartech-lab/e2e-casebook/blob/main/docs/test-hooks.md) for seeding data, injecting faults and controlling the clock.
- Each case is solved several ways in Playwright. Every approach is scored against bugs planted into the app, 10 runs per bug, so a test that only sometimes fails doesn't count as a catch.
- [12 worked solutions](https://github.com/bartech-lab/e2e-casebook/tree/main/solutions), 3 to 5 approaches each, with scores and trade-offs. In 5 of 11 scored cases no single approach catches every planted bug.
- An [AI-agent benchmark](https://github.com/bartech-lab/e2e-casebook/tree/main/solutions/benchmark) on the same cases: what coding agents test, miss and get wrong.

## Tools I built

**[dotfiles](https://github.com/bartech-lab/dotfiles)**: my macOS and Arch Linux setup, from one installer that is safe to re-run. It contains:

- a local LLM server: a 27B model on one consumer GPU, behind [a proxy](https://github.com/bartech-lab/dotfiles/blob/main/linux/bin/bonsai-cc-proxy.py) that keeps two large sessions from crashing it (58 tests)
- hourly git sync across machines
- a monitor that reports failed background services

Also: [lcw-dashboard](https://github.com/bartech-lab/lcw-dashboard), a local crypto dashboard in one Go binary, and [agents-usage-dashboard](https://github.com/bartech-lab/agents-usage-dashboard), AI coding assistant usage limits in one view (a Go rewrite of [AgentsUsageDashboard](https://github.com/konradozog-debug/AgentsUsageDashboard)).

## Volunteering

**[Tokens for Good](https://tokensforgood.ai/)**: research on nonprofits' measured impact, run on spare AI capacity. Gold contributor: 225 contributions, 20.1M tokens, 100% acceptance (2026-10-30).

## Contact

[LinkedIn](https://www.linkedin.com/in/bkow/)
