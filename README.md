# GitHub Workflow – 43030 Professional Practice in Computing

A student portfolio project demonstrating GitHub Actions automation, YAML workflow configuration, and automated file updates using `GITHUB_TOKEN`.

---

## Project Overview

This repository was built as part of Lecture 2 practical activities for 43030 Professional Practice in Computing at UTS.

It demonstrates:
- GitHub repository setup and structure
- Basic HTML file creation and GitHub Pages deployment
- YAML workflow configuration using GitHub Actions
- Automated updates to `index.html` on every push
- Automated commit logging to `README.md`
- Authenticated commits using `GITHUB_TOKEN`

---

## Repository Structure

```
/
├── .github/
│   └── workflows/
│       └── main.yml       ← GitHub Actions workflow
├── index.html             ← Web page (auto-updated on push)
└── README.md              ← This file (auto-logged on push)
```

---

## How the Workflow Works

When any team member pushes to the `main` branch:

1. GitHub Actions checks out the repository
2. The workflow detects which GitHub user triggered the push (`github.actor`)
3. A `<p>` tag is appended to `index.html` with the actor's name and timestamp
4. A log entry is appended to `README.md` with the actor, timestamp, and short commit hash
5. All changes are committed and pushed back using `GITHUB_TOKEN`

---

## Automated Commit Log

<!-- Workflow log entries will be appended below this line -->

### Updated by rairoy on 2026-06-09 21:03:29 [Commit: 4a27871]
### Updated by rairoy on 2026-06-09 21:08:56 [Commit: f2ef628]
### Updated by rairoy on 2026-06-09 21:21:54 [Commit: 49c66b7]
### Updated by rairoy on 2026-06-09 21:23:32 [Commit: a8901ff]
