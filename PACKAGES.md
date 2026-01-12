# Packages included in the installer

This document explains the packages included in each profile of `scripts/setup-termux.sh`. Edit the script if you want to add/remove items.

Profiles
- minimal — smallest set of tools a new learner needs to follow the lessons.
- recommended — minimal + common development and convenience tools.
- full — recommended + compilers, build tools, proot support and extras.

Packages and why they're useful
- git — version control; for cloning the repo and submitting contributions.
- openssh — ssh client/server (ssh, sshd).
- curl — fetch HTTP resources; often used in examples.
- wget — download files from the web.
- nano — simple terminal text editor friendly for beginners.
- vim — more powerful editor for users who want it.
- python — scripting and running many beginner-friendly examples.
- nodejs — javascript runtime; useful for many modern tools.
- termux-api — access Android device features from Termux (camera, battery, etc.).
- coreutils — common GNU utilities.
- unzip / zip — archive tools.
- jq — JSON processor (useful for many examples).
- tmux — terminal multiplexer for managing sessions.
- htop — interactive process viewer.
- rsync — efficient file sync/backup.
- clang / make / pkg-config — compilers and build tools (for people who need to build native code).
- proot-distro — run other distributions inside Termux (advanced).
- git-lfs — large file support for git (optional).
- gnupg — signing, key management.
- neofetch — system info display (cosmetic; optional).

If you want a different set, edit `scripts/setup-termux.sh` and change the arrays near the top.