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

**[dotfiles](https://github.com/bartech-lab/dotfiles)**: everything my macOS and Arch Linux machines run, from one idempotent installer with a dry-run mode and a doctor command.

- A local LLM server setup: systemd units for a 27B model on one consumer GPU, plus [a proxy](https://github.com/bartech-lab/dotfiles/blob/main/linux/bin/bonsai-cc-proxy.py) that adapts Claude Code and other agent requests to it and gates admission to its shared KV cache, so two large sessions can't crash it. The proxy has 58 tests.
- Hourly git auto-sync and a heartbeat monitor that reports failed services, with retries and logs.
- 26 test suites for the scripts, plus shellcheck and syntax checks by shebang.

Smaller: [lcw-dashboard](https://github.com/bartech-lab/lcw-dashboard) (a local crypto dashboard, one Go binary) and [agents-usage-dashboard](https://github.com/bartech-lab/agents-usage-dashboard) (AI assistant usage limits in one view, a Go rewrite of [AgentsUsageDashboard](https://github.com/konradozog-debug/AgentsUsageDashboard)).

## Volunteering

**[Tokens for Good](https://tokensforgood.ai/)**: research on nonprofits' measured impact, run on spare AI capacity. Gold contributor: 225 contributions, 20.1M tokens, 100% acceptance (2026-10-30).

## Contact

[LinkedIn](https://www.linkedin.com/in/bkow/)
