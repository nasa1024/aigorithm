# AIGorithm: Algorithm Practice with Codex CLI and VS Code

For the Chinese version, see `README-zh.md`.

This repository is designed for practicing algorithms one problem at a time with Codex CLI inside VS Code. It scaffolds tasks, you implement solutions, and Codex evaluates with structured feedback and suggestions.

## Overview
- Purpose: Practice algorithms in Go and Python, guided by Codex CLI.
- Flow: You request → Codex proposes a problem and scaffolds → You implement → Run tests → Ask Codex to evaluate → Codex generates feedback and `doc.md`.
- Scope: Sorting, searching, data structures, recursion, greedy, DP, graphs, trees, etc.

## Repository Structure
- `golang/` — Go implementations organized by categories (e.g., `sorting/`, `searching/`, `dp/`).
- `python/` — Python implementations organized similarly.
- `templates/` — Language‑specific templates used to scaffold new problems.
- `solutions/` — Reference solutions and best practices.
- `docs/` — Learning notes, analyses, and evaluations.
 
## Languages
- JavaScript/TypeScript: `javascript/`, `typescript/` — run with `node`/`ts-node`, test with `npm test` (Jest/Mocha/Vitest).
- Java: `java/` — Maven `mvn test` or Gradle `./gradlew test`.
- C++: `cpp/` — build with `g++` or CMake; optional `ctest`.
- Rust: `rust/` — `cargo run` / `cargo test`.
- C# (.NET): `csharp/` — `dotnet run` / `dotnet test`.
- Details for commands, style, and tests are summarized in `AGENTS.md`.

## Workflow with VS Code + Codex
- Open the folder in VS Code.
- Use Codex CLI (in the integrated terminal) to converse: describe what you want to learn/problem preference and ask Codex to scaffold.
- Codex creates the folder, starter files, and tests; you implement the core function.
- Run tests locally; iterate with Codex for hints or debugging.
- Request evaluation; Codex writes an assessment and suggestions (e.g., `docs/<topic>/doc.md`).

## Typical Session
1) Ask Codex for a problem (level/topic).
2) Codex scaffolds: `golang/<category>/<problem>/` with template and tests.
3) Implement core logic.
4) Run tests locally.
5) Request evaluation; Codex generates feedback + `doc.md`.

Example (Go, Bubble Sort):
- Path: `golang/sorting/bubble_sort/`
- Implement `bubbleSort(nums []int) []int` in `bubble_sort.go`, run `go test -v` in that folder.

## Notes
- This repo follows the guidance in `AGENTS.md` for structure, coding/testing standards, and evaluation.
- Use `gofmt` for Go and `black/autopep8` for Python formatting when applicable.
- Prefer meaningful names and include concise comments where they add clarity.
