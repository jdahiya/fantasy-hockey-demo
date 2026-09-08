# Fantasy Hockey — Live Demo

A **static, backend-free demo** of the Fantasy Hockey app (a Yahoo-Fantasy-style NHL fantasy app with full player stats and live game tracking).

**▶ Live site: https://jdahiya.github.io/fantasy-hockey-demo/**

Sign in with any email/password, then open the pre-made **Demo League** (or click *Try a demo league*). You can browse:

- **Players** — all 1,258 NHL players with real 2025-26 stats, filterable by position/team/availability and sortable by any stat.
- **My Team** — a drafted roster grouped by position slots.
- **Matchup / League / Live / Draft / Research** — the full app UI.

## How it works

This is the compiled web client from a private monorepo, built in **demo mode**: an in-browser mock serves a snapshot of real data captured from the app's Rust backend, so the entire UI is clickable with no server. It's read-only — lineup edits and other write actions are simulated locally.

The full app also ships native clients (iOS/macOS via SwiftUI, Android via Kotlin/Compose, Windows via WinUI 3, all over a shared C++ core) and a Rust service that ingests the public NHL API and tracks live games. Those live in the private source repository.

Deployed to GitHub Pages by [.github/workflows/pages.yml](.github/workflows/pages.yml).
