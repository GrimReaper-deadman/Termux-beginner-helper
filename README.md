# Termux First Steps

A beginner-friendly collection of lessons, scripts and examples to help new Termux users get started safely and confidently.

This repo now includes an opinionated installer script that can install different package profiles for learners:
- minimal — core tools to follow lessons
- recommended — minimal + commonly useful developer tools
- full — compilers, build tools and extras

Quick start (for learners)
1. Install Termux from F-Droid (recommended) or follow the official Termux distribution instructions.
2. Clone this repo:
   - git clone https://github.com/GrimReaper-deadman/Termux-beginner-helper.git

   - cd <repo>
3. Review the installer and run it:
   - bash scripts/setup-termux.sh --profile recommended
   - or preview with: bash scripts/setup-termux.sh --list
   - dry-run: bash scripts/setup-termux.sh --profile full --dry-run
   - skip confirmation: bash scripts/setup-termux.sh --profile full --yes

Notes & safety
- Always review any script before running it. This script uses Termux package manager (`pkg`) and installs only user-space packages. It does not require root.
- Use `--list` to see what packages each profile includes.
- The package lists are in `scripts/setup-termux.sh` and explained in `PACKAGES.md`.

Repository structure
- README.md — this file
- lessons/ — lesson files
- scripts/ — setup script (updated to support profiles)
- PACKAGES.md — explanations for the package lists
- LESSON_TEMPLATE.md — template for adding new lessons
- CONTRIBUTING.md — contribution guide
- LICENSE — MIT license

Next suggestions
- I can add a "dotfiles" lesson showing how to back up and restore configuration files to your GitHub repo.
- I can add a CI check that validates lesson frontmatter and runs a simple linter on Markdown.
- I can produce pre-made lessons for "shell basics", "git for beginners", and "SSH + keys".

Tell me which lessons or packages you want added or removed, and whether you want the installer to be strictly non-interactive for automated provisioning.