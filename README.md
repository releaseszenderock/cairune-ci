# Cairune CI

Quality gate runners for Cairune.

This repository holds **only CI workflows**. The application source is private: each run
fetches it with a read-only deploy key and runs the Linux and Windows gate (format, lint,
Clippy, Rust check, typecheck, generated bindings, tests, build). Runs are started by hand
by the maintainer; nothing here runs on pushes or pull requests.

Workflows:

- `gate.yml`: the Linux and Windows quality gate (format, lint, Clippy, Rust check, typecheck,
  generated bindings, tests, build).
- `build.yml`: distribution packaging (SHR-007). For the selected packages (Windows NSIS, unsigned
  MSIX, Linux deb, strict snap) it fetches and verifies the pinned engines, builds with the
  channel overlay, names, checksums and secret-scans each package, installs it on a fresh runner,
  launches it with `--smoke-test --smoke-engines`, checks that the installation is unchanged and
  that application data lands in the channel's location, and uninstalls it. Packages are unsigned
  and kept for a few days only; nothing is published.
