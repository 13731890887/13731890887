# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a **GitHub Profile README repository** - a single-file portfolio that displays on the user's GitHub profile page (https://github.com/13731890887).

## Project Structure

```
.
├── README.md    # The main GitHub profile README
└── .git/        # Git repository
```

**Important:** This repository contains only a README.md file. It is not a software project with code, tests, or build processes. The README is written in Markdown with HTML alignment tags.

## Purpose

The README.md serves as a personal portfolio page showcasing:
- User identity (Seqi, AI Researcher)
- Tech stack and skills
- Learning roadmap
- GitHub activity links

## Design Philosophy

**Zero External Dependencies:** The current design intentionally uses no external images or services to ensure maximum compatibility and avoid loading issues. All visual elements are created with:
- Plain text
- Emoji
- Unicode box-drawing characters (╔╗╚╝║─┼┬┴┌┐└┘)
- Markdown formatting

## Common Operations

### Updating the Profile
```bash
# Edit the README
vim README.md

# Commit changes
git add README.md
git commit -m "Description of changes"

# Push to GitHub (note: may need HTTP/1.1 for this repository)
git -c http.version=HTTP/1.1 push
```

### Viewing Changes
After pushing, visit https://github.com/13731890887 to see the updated profile. GitHub caches profile READMEs, so changes may take a few minutes to appear.

### Hard Refresh
If changes don't appear:
- Browser: Ctrl+Shift+R (Windows/Linux) or Cmd+Shift+R (Mac)
- Or add `?nocache=1` to the URL

## Known Issues

### Push Failures
Git pushes sometimes fail with "Error in the HTTP2 framing layer". Use HTTP/1.1:
```bash
git -c http.version=HTTP/1.1 push
```

### External Images
Previous versions used external image services (badgen.net, shields.io, vercel.app) which often failed to load. The current zero-dependency design avoids these issues entirely.

## Content Guidelines

- All data should be real (no placeholder emails or fake information)
- User's GitHub username is `seqi`
- Repository name is also `13731890887`
- Focus: Deep Learning, CNN, RNN, LSTM, Transformer, BERT, GPT
- Primary languages: Python, C++
- Frameworks: PyTorch, TensorFlow
