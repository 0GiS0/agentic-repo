# 🤖 Agentic Repo

<div align="center">

[![YouTube Channel Subscribers](https://img.shields.io/youtube/channel/subscribers/UC140iBrEZbOtvxWsJ-Tb0lQ?style=for-the-badge&logo=youtube&logoColor=white&color=red)](https://www.youtube.com/c/GiselaTorres?sub_confirmation=1)
[![GitHub followers](https://img.shields.io/github/followers/0GiS0?style=for-the-badge&logo=github&logoColor=white)](https://github.com/0GiS0)
[![LinkedIn Follow](https://img.shields.io/badge/LinkedIn-Follow-blue?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/giselatorresbuitrago/)
[![X Follow](https://img.shields.io/badge/X-Follow-black?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/0GiS0)

**🇪🇸 [Leer en Español](README.es.md)**

</div>

---

Hey developer 👋🏻! This repository contains a collection of **reusable GitHub workflows** powered by **GitHub Copilot CLI** for intelligent automation of your repositories.

## ✨ Features

- **✍️ Issue Quality Enhancer** — Automatically improves issue titles and bodies, translates to English, adds structure and relevant code references
- **🏷️ Smart Labeler** — Analyzes issues and PRs to assign the most appropriate labels
- **💡 Copilot Suggester** — Scans your codebase and creates discussion ideas for improvements (security, performance, UX, etc.)
- **🏷️✨ Label Beautifier** — Modernizes all your labels with emojis, descriptions, and consistent colors
- **📝 Continuous Documentation** — Improves README fragments and API docs as code evolves; nudges PR authors when explanations drift from the actual implementation
- **🚀 Workflow Installer** — Deploy these workflows to multiple repos with a single click

## 🛠️ Technologies

- GitHub Actions
- GitHub Copilot CLI
- GitHub MCP Server
- Playwright MCP Server (for UI analysis)

## 📋 Prerequisites

- GitHub account with **Copilot access**
- A **Personal Access Token (PAT)** with Copilot permissions stored as `COPILOT_PAT` secret

## 🚀 Installation

### Option 1: Use as Reusable Workflows (Recommended)

Copy the caller workflows from `caller-workflows/` to your repo's `.github/workflows/`:

```bash
# Clone this repo
git clone https://github.com/0GiS0/agentic-repo.git

# Copy the caller workflows you want
cp agentic-repo/caller-workflows/*.yml your-repo/.github/workflows/
```

Each caller is ~15 lines and references the main logic here, so you always get the latest version.

### Option 2: Use the Workflow Installer

1. Go to **Actions** → **🚀 Workflow Installer**
2. Enter target repos (comma-separated): `repo1, repo2, org/repo3`
3. Choose which workflows to install
4. Select whether to create a PR or push directly
5. Run!

### Option 3: Copy Full Workflows

Copy the workflows directly from `.github/workflows/` if you prefer full control.

## 💻 Usage

### Issue Quality Enhancer
Triggers automatically when an issue is opened. Enhances title, body, adds labels.

### Smart Labeler
Triggers on issue/PR open or edit. Analyzes content and assigns appropriate labels.

### Copilot Suggester
Run manually from Actions tab. Analyzes your codebase and creates discussion ideas.

### Label Beautifier
Run manually. Use `dry_run: true` first to preview changes.

### Continuous Documentation
Triggers automatically on PRs that modify code files. Compares changes against existing README sections and API docs, suggests updates, and leaves a review comment when documentation drifts from the implementation.

## 📁 Project Structure

```
agentic-repo/
├── .github/
│   └── workflows/
│       ├── issue-quality-enhancer.yml    # Reusable workflow
│       ├── smart-labeler.yml             # Reusable workflow
│       ├── the-suggester-discussion-mode.yml  # Reusable workflow
│       ├── label-beautifier.yml          # Reusable workflow
│       ├── continuous-docs.yml            # Reusable workflow
│       └── workflow-installer.yml        # Installer utility
├── caller-workflows/                     # Lightweight callers for other repos
│   ├── issue-quality-enhancer.yml
│   ├── smart-labeler.yml
│   ├── the-suggester-discussion-mode.yml
│   ├── label-beautifier.yml
│   └── continuous-docs.yml
└── README.md
```

## ⚙️ Required Setup in Target Repos

Add this secret to any repo using these workflows:
- `COPILOT_PAT` — GitHub PAT with Copilot access

---

## 🌐 Follow Me

<div align="center">

[![YouTube Channel Subscribers](https://img.shields.io/youtube/channel/subscribers/UC140iBrEZbOtvxWsJ-Tb0lQ?style=for-the-badge&logo=youtube&logoColor=white&color=red)](https://www.youtube.com/c/GiselaTorres?sub_confirmation=1)
[![GitHub followers](https://img.shields.io/github/followers/0GiS0?style=for-the-badge&logo=github&logoColor=white)](https://github.com/0GiS0)
[![LinkedIn Follow](https://img.shields.io/badge/LinkedIn-Follow-blue?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/giselatorresbuitrago/)
[![X Follow](https://img.shields.io/badge/X-Follow-black?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/0GiS0)

</div>
