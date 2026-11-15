# Jeremy Mackey

Software Engineer

## Selected projects

[Event Review · Python](https://github.com/jmac4909/event-review-agent) · [JM Ops Agent · Java](https://github.com/jmac4909/jm-ops-agent) · [PaneFleet · Node.js](https://github.com/jmac4909/PaneFleet) · [Kronos · TypeScript](https://github.com/jmac4909/Kronos)

Source, architecture notes, and local setup are linked below. Screenshots show real application interfaces with demo data; select an image to explore a project.

### [Event Review](https://github.com/jmac4909/event-review-agent)

A Python/FastAPI, PostgreSQL, and React prototype for reviewing safety alerts. A custom agent loop combines event evidence, scoped retrieval, and supervisor-approved guidance. Correcting one event does not automatically create a rule for future events. Regional row-level security, expiring work claims, and bounded retries keep data and worker ownership explicit.

<a href="https://jmac.page/#event-review"><img src="https://jmac.page/assets/event-review.png" alt="Event Review dashboard with synthetic regional alerts, a Mock agent assessment, and supervisor review controls" width="640"></a>

[Watch demo](https://www.loom.com/share/253ef7d8a36a49eba6e7cbc559d3cd96) · [Architecture](https://github.com/jmac4909/event-review-agent/blob/main/docs/architecture.md) · [Feedback walkthrough](https://github.com/jmac4909/event-review-agent/blob/main/docs/walkthrough.md) · [Verification](https://github.com/jmac4909/event-review-agent/blob/main/docs/verification.md) · [Run locally](https://github.com/jmac4909/event-review-agent#run)

Uses synthetic detector metadata, not camera footage. Mock runs offline after setup; the repository also documents live Claude evaluations.

### [JM Ops Agent](https://github.com/jmac4909/jm-ops-agent)

A Java 21 / Spring Boot proof of concept for read-only service investigations. It traces failures across services and presents a diagnosis with supporting evidence. The local mock demo runs without enterprise credentials, external services, or model usage.

<a href="projects/jm-ops-agent.md"><img src="assets/jmops-investigation-result.png" alt="JM Ops Agent diagnosis with supporting evidence from the local mock demo" width="640"></a>

[Architecture](https://github.com/jmac4909/jm-ops-agent/blob/main/docs/architecture.md) · [Investigation design](https://github.com/jmac4909/jm-ops-agent/blob/main/docs/adaptive-investigations.md) · [Run the mock demo](https://github.com/jmac4909/jm-ops-agent#run-the-zero-connectivity-demo)

### [PaneFleet](https://github.com/jmac4909/PaneFleet)

A Node.js dashboard for supervising terminal-based coding agents from desktop or phone. It adds project context, durable work queues, and exact-pane input delivery to tmux. Uncertain actions stay visible for review rather than being retried blindly.

<a href="projects/panefleet.md"><img src="assets/panefleet-workspace.png" alt="PaneFleet terminal workspace with synthetic sessions" width="640"></a>

[Architecture](https://github.com/jmac4909/PaneFleet/blob/main/docs/architecture.md) · [Safety model](https://github.com/jmac4909/PaneFleet/blob/main/docs/safety-model.md) · [Run locally](https://github.com/jmac4909/PaneFleet#quick-start)

### [Kronos](https://github.com/jmac4909/Kronos)

A TypeScript VS Code extension that brings Jira, GitLab, Jenkins, and SonarQube context into a terminal-first workflow. Provider access is read-only; the developer controls execution and submission. No third-party runtime dependencies.

<a href="projects/kronos.md"><img src="assets/kronos-board.png" alt="Kronos Jira work webview with synthetic tickets" width="640"></a>

[Product contract](https://github.com/jmac4909/Kronos/blob/main/docs/terminal-first-product-contract.md) · [State ownership](https://github.com/jmac4909/Kronos/blob/main/docs/state-ownership.md) · [Try the preview](https://github.com/jmac4909/Kronos#try-it-locally)

Kronos is preview software; JM Ops Agent is a proof of concept.

## Application showcases

These projects have private source code. The linked write-ups explain their workflows and engineering.

### [Cribbage Tournament Review](projects/cribbage.md)

A phone-first Python/web app for turning handwritten score-card photos into reviewed tournament results. Combines AI-assisted reading, cross-card validation, and focused correction tools.

<a href="projects/cribbage.md"><img src="assets/cribbage-results.png" alt="Cribbage standings calculated from a validated synthetic tournament" width="640"></a>

### [Multiplayer Poker](projects/poker.md)

A real-time poker app built with Elixir/Phoenix, PostgreSQL, and Expo/React Native. The server owns game state and tournament progression; web and mobile clients share the same backend.

<a href="projects/poker.md"><img src="assets/poker-lobby.png" alt="Poker lobby with demo tournaments" width="640"></a>
