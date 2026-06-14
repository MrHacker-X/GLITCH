<div align="center">

<img src="https://glitch.vritrasec.com/assets/img/glitch.png" alt="Glitch AI Engine" width="80" height="80">

# Glitch AI Engine

**Linux-native terminal with integrated Glitch AI**

Community hub for bug reports, feature requests, and product feedback

[![Version](https://img.shields.io/badge/version-v0.8.5--stable-2d6a4f?style=for-the-badge)](https://glitch.vritrasec.com/download/)
[![Platform](https://img.shields.io/badge/platform-Linux%20amd64%20%7C%20arm64-4a5568?style=for-the-badge)](https://glitch.vritrasec.com/docs/installation/)
[![Website](https://img.shields.io/badge/website-glitch.vritrasec.com-2d6a4f?style=for-the-badge)](https://glitch.vritrasec.com/)

[Website](https://glitch.vritrasec.com/) · [Download](https://glitch.vritrasec.com/download/) · [Documentation](https://glitch.vritrasec.com/docs/) · [VritraSec](https://vritrasec.com)

</div>

---

## Table of Contents

- [About This Repository](#about-this-repository)
- [Overview](#overview)
- [Screenshots](#screenshots)
- [Features](#features)
- [Supported AI Models](#supported-ai-models)
- [Download & Installation](#download--installation)
- [Community & Support](#community--support)
- [Resources](#resources)
- [System Requirements](#system-requirements)
- [Maintainer](#maintainer)

---

## About This Repository

This repository serves as the **official community hub** for [Glitch AI Engine](https://glitch.vritrasec.com/). It provides a single, structured channel for users to engage with the product team.

| Purpose | Description |
|---------|-------------|
| Bug reports | Report crashes, regressions, and unexpected behavior |
| Feature requests | Propose workflow improvements and new capabilities |
| Questions | Installation, configuration, and Glitch AI setup support |
| Issue tracking | Follow known issues and release fixes |

> **Note:** Application source code is not hosted in this repository. Downloads, release builds, and full documentation are maintained on the [official website](https://glitch.vritrasec.com/).

---

## Overview

**Glitch AI Engine** is a production desktop terminal for Linux, developed by **Alex Butler** at **[Vritra Security Organization](https://vritrasec.com)** (VritraSec).

Unlike chat-first terminal wrappers, Glitch runs your **native system shell** (bash, zsh, or your configured login shell) inside a modern workspace augmented by a built-in **Glitch AI** assistant panel.

| Property | Value |
|----------|-------|
| Release | `v0.8.5-stable` |
| Platform | Linux, amd64 (x86_64) · arm64 (AArch64) |
| Application ID | `com.vritrasec.glitch` |
| CLI binary | `glitch` |
| Configuration | `~/.config-vritrasecz/Glitch/` |
| AI integration | Glitch AI (Gemini API key required) |
| Default model | `gemini-2.5-flash-lite` |

---

## Screenshots

<details open>
<summary><strong>Terminal session with Glitch AI panel</strong></summary>
<br>

<div align="center">
  <img src="https://glitch.vritrasec.com/assets/img/terminal/glitch-screenshot.png" alt="Glitch AI Engine terminal with integrated AI panel" width="920">
  <p><sub>v0.8.5-stable, live shell session with workspace-aware AI diagnostics</sub></p>
</div>

</details>

<details>
<summary><strong>Product overview</strong></summary>
<br>

<div align="center">
  <img src="https://glitch.vritrasec.com/assets/img/og-image/og-home-glitch.webp" alt="Glitch AI Engine product overview" width="920">
</div>

</details>

<details>
<summary><strong>Documentation & theme gallery</strong></summary>
<br>

<div align="center">
  <img src="https://glitch.vritrasec.com/assets/img/og-image/og-docs-glitch.webp" alt="Glitch AI Engine documentation and themes" width="920">
  <p><sub><a href="https://glitch.vritrasec.com/docs/themes/">View all 10 themes in the documentation</a></sub></p>
</div>

</details>

---

## Features

### Glitch AI

| Capability | Description |
|------------|-------------|
| **Send to AI** | Select terminal output → right-click → Send to AI. Opens the panel, prefixes `/shell`, and focuses input for diagnostics. |
| **Chat mode** | General workspace assistance with streaming responses and session memory. |
| **Shell mode** | Command-output analysis via `/shell` for logs, build failures, and runtime errors. |
| **File context** | Attach workspace files with `@filename` mentions in the AI panel. |

Documentation: [AI Assistant](https://glitch.vritrasec.com/docs/ai-assistant/) · [Send to AI guide](https://glitch.vritrasec.com/docs/ai-assistant/#send-to-ai)

### Terminal workspace

| Capability | Description |
|------------|-------------|
| Native shell | Runs your real login shell, not a simulated environment |
| Tabs & splits | Multi-tab layout with horizontal and vertical split panes |
| Session restore | Tabs, split tree, working directories, and themes persist across restarts |
| Command Palette | 18 system-administration quick commands (`Ctrl`+`Shift`+`P`) |
| Themes | 10 curated palettes including Vritra Matrix (default) and Ghost Glitch |
| Productivity | 5,000-line scrollback · clickable hyperlinks · read-only and full-screen modes |

Documentation: [Features](https://glitch.vritrasec.com/docs/features/) · [Keyboard shortcuts](https://glitch.vritrasec.com/docs/keyboard-shortcuts/) · [Command Palette](https://glitch.vritrasec.com/docs/command-palette/)

---

## Supported AI Models

Model availability is synchronized from the official endpoint:  
`https://glitch.vritrasec.com/config/models.json`

| Model | Role |
|-------|------|
| `gemini-2.5-flash-lite` | **Default** |
| `gemini-flash-latest` | Stable |
| `gemini-3.5-flash` | Stable |
| `gemini-flash-lite-latest` | Stable |
| `gemini-3-flash-preview` | Stable |
| `gemini-3.1-flash-lite-preview` | Stable |
| `gemini-3.1-flash-lite` | Stable |
| `gemini-2.5-flash` | Stable |
| `gemma-4-31b-it` | Stable |
| `gemma-4-26b-a4b-it` | Stable |

---

## Download & Installation

Official builds are distributed via the VritraSec CDN.

| Architecture | Debian package | Standalone binary |
|:------------:|:--------------|:-----------------|
| **amd64** | [glitch_0.8.5_amd64.deb](https://cdn.vritrasec.com/glitch/amd64/glitch_0.8.5_amd64.deb) | [glitch-v0.8.5-linux-amd64](https://cdn.vritrasec.com/glitch/amd64/glitch-v0.8.5-linux-amd64) |
| **arm64** | [glitch_0.8.5_arm64.deb](https://cdn.vritrasec.com/glitch/arm64/glitch_0.8.5_arm64.deb) | [glitch-v0.8.5-linux-arm64](https://cdn.vritrasec.com/glitch/arm64/glitch-v0.8.5-linux-arm64) |

**Quick install (amd64 .deb):**

```bash
sudo dpkg -i glitch_0.8.5_amd64.deb
glitch -v
```

Further guidance: [Download page](https://glitch.vritrasec.com/download/) · [Installation guide](https://glitch.vritrasec.com/docs/installation/)

---

## Community & Support

Feedback is welcome. Before submitting an issue, consult the [documentation](https://glitch.vritrasec.com/docs/), installation steps, AI setup, and feature references are documented there.

### Submit an issue

[**Open a new issue →**](../../issues/new)

| Category | Use when | Suggested label |
|----------|----------|-----------------|
| Bug report | A feature fails, crashes, or behaves incorrectly | `bug` |
| Feature request | A capability or workflow improvement is needed | `enhancement` |
| Question | Help with install, config, API key, or usage | `question` |

<details>
<summary><strong>Bug report template</strong></summary>

```markdown
**Version:** v0.8.5-stable
**OS / distribution:** e.g. Kali Linux, Ubuntu 24.04
**Architecture:** amd64 / arm64
**Install method:** .deb / binary

**Summary:**
Brief description of the issue.

**Expected behavior:**
What should have happened.

**Actual behavior:**
What happened instead.

**Steps to reproduce:**
1.
2.
3.

**Attachments:**
Screenshots, logs, or terminal output (if applicable).

**Additional context:**
AI panel involved: yes / no
Active theme: e.g. Vritra Matrix
```

</details>

<details>
<summary><strong>Feature request template</strong></summary>

```markdown
**Summary:**
One-line description of the proposed improvement.

**Problem statement:**
What workflow is currently slow, missing, or inefficient.

**Proposed solution:**
Focused description of the desired behaviour.

**Alternatives considered:**
Workarounds or partial solutions already attempted.

**Impact:**
How this benefits Linux terminal users.
```

</details>

### Out of scope for this repository

- Application source code pull requests
- Private security disclosures, contact [VritraSec](https://vritrasec.com) directly
- Website or documentation corrections, submit as a general `question` issue

---

## Resources

### Official endpoints

| Resource | URL |
|----------|-----|
| Website | https://glitch.vritrasec.com/ |
| Documentation | https://glitch.vritrasec.com/docs/ |
| Download | https://glitch.vritrasec.com/download/ |
| About | https://glitch.vritrasec.com/about/ |
| Privacy policy | https://glitch.vritrasec.com/privacy/ |
| Update manifest | https://glitch.vritrasec.com/config/update.json |
| Models configuration | https://glitch.vritrasec.com/config/models.json |

### Documentation index

| Guide | Link |
|-------|------|
| Getting Started | https://glitch.vritrasec.com/docs/getting-started/ |
| Installation | https://glitch.vritrasec.com/docs/installation/ |
| Features | https://glitch.vritrasec.com/docs/features/ |
| AI Assistant | https://glitch.vritrasec.com/docs/ai-assistant/ |
| Command Palette | https://glitch.vritrasec.com/docs/command-palette/ |
| Keyboard Shortcuts | https://glitch.vritrasec.com/docs/keyboard-shortcuts/ |
| Themes | https://glitch.vritrasec.com/docs/themes/ |
| Menus | https://glitch.vritrasec.com/docs/menus/ |
| Advanced | https://glitch.vritrasec.com/docs/advanced/ |

---

## System Requirements

| Requirement | Specification |
|-------------|---------------|
| Operating system | Linux (Debian-based distributions recommended for `.deb` installs) |
| Architecture | amd64 (x86_64) or arm64 (AArch64) |
| Shell | bash, zsh, or any configured login shell |
| Glitch AI | Valid Gemini API key, configured under **Settings → AI Core Setup** |
| Desktop environment | GTK4 / libadwaita compatible display server |

---

## Maintainer

| | |
|---|---|
| **Developer** | Alex Butler |
| **Organization** | [Vritra Security Organization](https://vritrasec.com) |
| **Product** | Glitch AI Engine |
| **Current release** | v0.8.5-stable, initial stable release |

---

<div align="center">

<sub>Glitch AI Engine · Linux terminal with built-in intelligence</sub><br>
<sub>© 2026 Vritra Security Organization</sub>

</div>
