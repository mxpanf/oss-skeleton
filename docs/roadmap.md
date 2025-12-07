# Project Roadmap

This document outlines the development plan for `oss-skeleton`. Our goal is to provide the most robust, language-agnostic starting point for new projects.

**Legend:**
- ✅ Completed
- 🚧 In Progress
- 🔮 Planned / Exploring

---

## Q4 2025: Foundation (v1.0)
*Focus: Stabilizing the core file structure and documentation.*

- ✅ Define the "Gold Standard" directory layout.
- ✅ Create GitHub Actions workflow for basic health checks.
- ✅ Implement standardized `.editorconfig` for cross-IDE compatibility.
- ✅ Write comprehensive `CONTRIBUTING.md` and `CODE_OF_CONDUCT.md`.
- 🚧 Create a landing page for the documentation (GitHub Pages).

## Q1 2026: Automation & Expansion
*Focus: Making the template smarter and more interactive.*

- 🔮 **Scripted Setup:** Add a `setup.sh` (or `init.js`) script to interactively rename the project and replace placeholders (Author, Year, Email).
- 🔮 **Language Variants:** Create branches for specific ecosystems:
    - `flavor/python` (adds `pyproject.toml`, `requirements.txt`)
    - `flavor/node` (adds `package.json`, `eslintrc`)
    - `flavor/go` (adds `go.mod`)
- 🔮 **Semantic Release:** Integrate automated versioning and changelog generation based on commit messages.

## Q2 2026: Community & Governance
*Focus: Scaling the project maintainability.*

- 🔮 Add a Governance model document for multi-maintainer projects.
- 🔮 Integrate "All Contributors" bot for automated credit.
- 🔮 Create a badge generator for the README.

---

## Long-term Vision

We aim to turn `oss-skeleton` into a CLI tool (`npx create-oss-project`) that dynamically generates this structure based on user input, rather than just being a static Git template.
