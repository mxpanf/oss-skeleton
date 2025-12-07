# Architecture Blueprint: OSS Skeleton

## 1. Design Philosophy

The `oss-skeleton` is built upon three core pillars designed to minimize friction for new Open Source projects:

1. **Zero-Config Start:** The template assumes reasonable defaults (e.g., VS Code settings, standard `.gitignore`) so developers can start coding immediately.

2. **Administrative Clarity:** Separating "meta" files (like docs, github workflows) from "source" code (`src/`) prevents root directory clutter.

3. **Compliance by Default:** Pre-including legal and community health files (`LICENSE`, `SECURITY`, `CODE_OF_CONDUCT`) ensures the repository is "good citizen" ready from day one.

## 2. Directory Strategy

The file tree is organized into functional zones:

```mermaid
graph TD
    Root[Project Root] --> Admin[Administrative Zone]
    Root --> Dev[Development Zone]
    Root --> Meta[Community Zone]

    Admin --> Configs[.editorconfig, .gitignore]
    Admin --> CI[.github/workflows]

    Dev --> Src[src/]
    Dev --> Tests[tests/]

    Meta --> Docs[docs/]
    Meta --> Legal[LICENSE, NOTICE]
    Meta --> Health[CONTRIBUTING, SECURITY]
````

### 2.1 The `docs/` Separation

We deliberately moved architectural assets and roadmaps into `docs/` to keep the root `README.md` focused on *usage* rather than *internals*. This follows the "Documentation as Code" approach, where documentation lives alongside the source but doesn't obstruct it.

## 3\. Workflow Integration

The skeleton is designed to trigger specific GitHub behaviors automatically:

  * **Issue Templates:** By placing YAML-frontmatter files in `.github/ISSUE_TEMPLATE/`, GitHub creates a guided UI for bug reporting.

  * **Security Policy:** The presence of `SECURITY.md` activates a specific "Security" tab in the repo interface.

  * **Discussion Links:** `CONTRIBUTING.md` is automatically suggested by GitHub when a user attempts to open a new PR.

## 4\. Future Extensibility

This structure is a baseline. It is intended to be extended:

  * **Monorepos:** The `src/` folder can be replaced with `packages/` for workspaces (npm/cargo/etc).

  * **Dockerization:** A `Dockerfile` and `docker-compose.yml` fit naturally at the root level without conflicting with existing configs.
