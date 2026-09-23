# Cairune CI

Quality gate runners for Cairune.

This repository holds **only CI workflows**. The application source is private: each run
fetches it with a read-only deploy key and runs the Linux and Windows gate (format, lint,
Clippy, Rust check, typecheck, generated bindings, tests, build). Runs are started by hand
by the maintainer; nothing here runs on pushes or pull requests.
