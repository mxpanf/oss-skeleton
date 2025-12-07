# OSS Skeleton

![License](https://img.shields.io/github/license/mxpanf/oss-skeleton?style=flat-square)
![Build Status](https://img.shields.io/github/actions/workflow/status/mxpanf/oss-skeleton/main.yml?style=flat-square&label=Build)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-orange.svg?style=flat-square)](CONTRIBUTING.md)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg?style=flat-square)](CODE_OF_CONDUCT.md)

> **A clean, universal directory structure and standard file baseline for seamless Open Source project starts.**

> [!IMPORTANT]
> **Disclaimer**
>
> These files are illustrative examples and may not represent the real project status. The structure is **unlicensed** and provided **"AS IS"**.
>
> For usage guidelines, please read the **README**. This message contains the only valid information regarding the project's status.

## Table of Contents

- [About](#about)
- [Features](#features)
- [Directory Structure](#directory-structure)
- [How to Use](#how-to-use)

## About

**OSS Skeleton** is a "zero-hassle" template for starting professional Open Source repositories. Instead of creating standard files from scratch or copying them from old projects, use this skeleton as a robust foundation.

It is designed to be **language-agnostic** (suitable for Python, JS, Go, Rust, etc.) and focuses on administrative clarity.

## Features

* **⚙️ Consistent Configs**: Includes a tuned `.editorconfig` and a robust `.gitignore` covering common OS and IDE temp files (Windows, macOS, VS Code, JetBrains).
* **📝 Ready-to-use Docs**: Pre-filled, professional templates for `LICENSE`, `CONTRIBUTING.md`, and `CODE_OF_CONDUCT.md`.
* **📂 Organized Structure**: A dedicated `docs/` folder for blueprints, roadmaps, and assets, keeping your root directory clean.
* **🛡️ Security First**: Includes a `SECURITY.md` policy template to establish a safe reporting channel from day one.

## 📂 Directory Structure

This skeleton provides the following file tree:

```text
.
├── .github/
│   ├── ISSUE_TEMPLATE/       # Templates for bug reports & features
│   ├── PULL_REQUEST_TEMPLATE.md
│   └── workflows/            # CI/CD pipelines
├── docs/                     # Documentation (concept, design)
│   ├── assets/               # Images, diagrams, logos
│   ├── architecture.md       # Technical blueprints
│   └── roadmap.md            # Future plans
├── src/                      # Source code (rename as needed)
├── tests/                    # Tests directory
├── .editorconfig             # Cross-editor consistency
├── .gitignore                # Global ignore rules
├── CHANGELOG.md              # Keep a Changelog standard
├── CODE_OF_CONDUCT.md        # Community standards
├── CONTRIBUTING.md           # Contribution guidelines
├── LICENSE                   # MIT License
├── NOTICE                    # Copyright notices
├── README.md                 # Project entry point
└── SECURITY.md               # Vulnerability reporting policy
````

## 🛠 How to Use

1.  **Click "Use this template"** at the top of the repository page to generate a new repo with this structure.
2.  **Clone** your new repository locally.
3.  **Perform the Checklist** below to personalize the repo.
4.  **Start Coding**: Place your source code in `src/` (or rename it to your package name).

### ✅ Post-Creation Checklist

After creating a new repository from this template, **you must update the following files** to match your project details:

  - [ ] **README.md**:
      - Replace badge links at the top (update `mxpanf/oss-skeleton` to your `user/repo`).
      - Update project title and description.
  - [ ] **LICENSE**:
      - Replace the author name and year.
      - *Optional:* Change the license text entirely if you are not using MIT.
  - [ ] **NOTICE**:
      - Replace with your name or organization.
  - [ ] **CHANGELOG.md**:
      - Update or reset the `[0.1.0]` entry for your first release.
  - [ ] **CONTRIBUTING.md**:
      - Update contact email (approx. line 23).
      - Update GitHub Issue links to your repository (approx. lines 29, 33).
  - [ ] **CODE\_OF\_CONDUCT.md**:
      - Update contact email for enforcement (approx. line 62).
  - [ ] **SECURITY.md**:
      - Update contact email for security reporting (approx. line 20).
  - [ ] *`.github`*:
      - Update github workflows & templates.
