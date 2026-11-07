# Horizzon

Building around **[aspaslabs.com](https://aspaslabs.com)**. Tools that feel like part of the system, not another layer of bloat. Powered by Linux (CachyOS), Rust, and too many terminal tabs. Soft spot for liminal aesthetics and old desktop UIs. Builds things for himself first, then shares them.

![Web](https://img.shields.io/badge/-Web-4285F4?style=flat-square&logo=google-chrome&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Electron](https://img.shields.io/badge/-Electron-47848F?style=flat-square&logo=electron&logoColor=white)
![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Bun](https://img.shields.io/badge/-Bun-000000?style=flat-square&logo=bun&logoColor=white)
![Rust](https://img.shields.io/badge/-Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Codex](https://img.shields.io/badge/-Codex-121212?style=flat-square&logo=data:image/svg%2Bxml%3Bbase64,PHN2ZyByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48dGl0bGU%2BT3BlbkFJPC90aXRsZT48cGF0aCBmaWxsPSJ3aGl0ZSIgZD0iTTIyLjI4MTkgOS44MjExYTUuOTg0NyA1Ljk4NDcgMCAwIDAtLjUxNTctNC45MTA4IDYuMDQ2MiA2LjA0NjIgMCAwIDAtNi41MDk4LTIuOUE2LjA2NTEgNi4wNjUxIDAgMCAwIDQuOTgwNyA0LjE4MThhNS45ODQ3IDUuOTg0NyAwIDAgMC0zLjk5NzcgMi45IDYuMDQ2MiA2LjA0NjIgMCAwIDAgLjc0MjcgNy4wOTY2IDUuOTggNS45OCAwIDAgMCAuNTExIDQuOTEwNyA2LjA1MSA2LjA1MSAwIDAgMCA2LjUxNDYgMi45MDAxQTUuOTg0NyA1Ljk4NDcgMCAwIDAgMTMuMjU5OSAyNGE2LjA1NTcgNi4wNTU3IDAgMCAwIDUuNzcxOC00LjIwNTggNS45ODk0IDUuOTg5NCAwIDAgMCAzLjk5NzctMi45MDAxIDYuMDU1NyA2LjA1NTcgMCAwIDAtLjc0NzUtNy4wNzI5em0tOS4wMjIgMTIuNjA4MWE0LjQ3NTUgNC40NzU1IDAgMCAxLTIuODc2NC0xLjA0MDhsLjE0MTktLjA4MDQgNC43NzgzLTIuNzU4MmEuNzk0OC43OTQ4IDAgMCAwIC4zOTI3LS42ODEzdi02LjczNjlsMi4wMiAxLjE2ODZhLjA3MS4wNzEgMCAwIDEgLjAzOC4wNTJ2NS41ODI2YTQuNTA0IDQuNTA0IDAgMCAxLTQuNDk0NSA0LjQ5NDR6bS05LjY2MDctNC4xMjU0YTQuNDcwOCA0LjQ3MDggMCAwIDEtLjUzNDYtMy4wMTM3bC4xNDIuMDg1MiA0Ljc4MyAyLjc1ODJhLjc3MTIuNzcxMiAwIDAgMCAuNzgwNiAwbDUuODQyOC0zLjM2ODV2Mi4zMzI0YS4wODA0LjA4MDQgMCAwIDEtLjAzMzIuMDYxNUw5Ljc0IDE5Ljk1MDJhNC40OTkyIDQuNDk5MiAwIDAgMS02LjE0MDgtMS42NDY0ek0yLjM0MDggNy44OTU2YTQuNDg1IDQuNDg1IDAgMCAxIDIuMzY1NS0xLjk3MjhWMTEuNmEuNzY2NC43NjY0IDAgMCAwIC4zODc5LjY3NjVsNS44MTQ0IDMuMzU0My0yLjAyMDEgMS4xNjg1YS4wNzU3LjA3NTcgMCAwIDEtLjA3MSAwbC00LjgzMDMtMi43ODY1QTQuNTA0IDQuNTA0IDAgMCAxIDIuMzQwOCA3Ljg3MnptMTYuNTk2MyAzLjg1NThMMTMuMTAzOCA4LjM2NCAxNS4xMTkyIDcuMmEuMDc1Ny4wNzU3IDAgMCAxIC4wNzEgMGw0LjgzMDMgMi43OTEzYTQuNDk0NCA0LjQ5NDQgMCAwIDEtLjY3NjUgOC4xMDQydi01LjY3NzJhLjc5Ljc5IDAgMCAwLS40MDctLjY2N3ptMi4wMTA3LTMuMDIzMWwtLjE0Mi0uMDg1Mi00Ljc3MzUtMi43ODE4YS43NzU5Ljc3NTkgMCAwIDAtLjc4NTQgMEw5LjQwOSA5LjIyOTdWNi44OTc0YS4wNjYyLjA2NjIgMCAwIDEgLjAyODQtLjA2MTVsNC44MzAzLTIuNzg2NmE0LjQ5OTIgNC40OTkyIDAgMCAxIDYuNjgwMiA0LjY2ek04LjMwNjUgMTIuODYzbC0yLjAyLTEuMTYzOGEuMDgwNC4wODA0IDAgMCAxLS4wMzgtLjA1NjdWNi4wNzQyYTQuNDk5MiA0LjQ5OTIgMCAwIDEgNy4zNzU3LTMuNDUzN2wtLjE0Mi4wODA1TDguNzA0IDUuNDU5YS43OTQ4Ljc5NDggMCAwIDAtLjM5MjcuNjgxM3ptMS4wOTc2LTIuMzY1NGwyLjYwMi0xLjQ5OTggMi42MDY5IDEuNDk5OHYyLjk5OTRsLTIuNTk3NCAxLjQ5OTctMi42MDY3LTEuNDk5N1oiLz48L3N2Zz4%3D)
![Cursor](https://img.shields.io/badge/-Cursor-000000?style=flat-square&logo=cursor&logoColor=white)
![Devin](https://img.shields.io/badge/-Devin-000000?style=flat-square&logo=windsurf&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Tauri](https://img.shields.io/badge/-Tauri-FFC131?style=flat-square&logo=tauri&logoColor=black)
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

## Start Here

- ✍️ **[abstract](https://github.com/fireflylabss/abstract)** — native Markdown notes editor built on Rust + GPUI
- 🎵 **[stillmusic](https://github.com/horizzon3507/stillmusic)** — black-and-white MPV CLI music player
- 📊 **[usagenometer](https://github.com/horizzon3507/usagenometer)** — AI usage meters in the terminal (+ beta GNOME Shell companion)
- <img src="ace-emoji.png" width="18" valign="middle" alt="ace"> **[ace](https://github.com/horizzon3507/ace)** — all-in-one Fluxer bot: moderation, info cards, per-server prefix

## Current Projects

### Public Projects

- 🗂️ **[fluboard](https://fluboard.hory.one)** — Catalog of Brazilian Fluxer communities and bots
- <img src="ace-emoji.png" width="18" valign="middle" alt="ace"> **[ace](https://github.com/horizzon3507/ace)** — all-in-one Fluxer bot: moderation, info cards, per-server prefix

### Music

- 🎵 **[stillmusic](https://github.com/horizzon3507/stillmusic)** — Local black-and-white MPV CLI music player
- 🎮 **[fragment](https://github.com/horizzon3507/fragment)** — Guess the song from a snippet that keeps growing — local music, terminal game

### Terminal Utilities

- 🧹 **[tend](https://github.com/horizzon3507/tend)** — Tends your machine: scans dead weight, cleans safely, backs up dotfiles
- 🔦 **[flashlog](https://github.com/horizzon3507/flashlog)** — Highlights errors, secrets, and stack traces in terminal output
- 📊 **[usagenometer](https://github.com/horizzon3507/usagenometer)** — AI usage meters in the terminal (`usg`)
- 🎙️ **[stfu](https://github.com/horizzon3507/stfu)** — Kill switch for all microphones: Rust CLI for PipeWire/WirePlumber
- 🩺 **[gitpulse](https://github.com/horizzon3507/gitpulse)** — Pulse-check every local repo: dirty trees, unpushed commits, stale branches, missing remotes

### Utilities

- 🔄 **[handoff](https://github.com/horizzon3507/handoff)** — Send files between devices over local Wi-Fi
- 🪄 **[SkillsByHory](https://github.com/horizzon3507/SkillsByHory)** — Agent skills by Hory: versioning, releases, AUR, local-first
- ⌨️ **[glyphic](https://glyphic.hory.one)** — Terminal-style image→ASCII studio: CRT viewport with zoom/pan, color mode, exports to PNG/SVG/TXT/HTML
- 🧭 **[exitq](https://github.com/horizzon3507/exitq)** — Extract CopyQ backups into ordered files
- ✍️ **[abstract](https://github.com/fireflylabss/abstract)** — Native Rust + GPUI Markdown notes editor

### Libs & Packages

- 🍋 **[Yuzuha](https://github.com/horizzon3507/yuzuha)** — TypeScript framework for Fluxer bots with typed commands and optional scripts
- 🧱 **[Flush](https://github.com/horizzon3507/Flush)** — Rust framework for Fluxer bots: Gateway WS + REST + command router, parity with @fluxerjs/core
- 📦 **[synara-aur](https://aur.archlinux.org/packages/synara)** — Unofficial AUR package for [Synara](https://trysynara.com) (AppImage)
- 📦 **[fluxter-aur](https://aur.archlinux.org/packages/fluxter)** — Unofficial AUR package for [fluxter](https://github.com/AIVirtuoso/fluxter), the TUI Fluxer client
- 📦 **[tardigrade-aur](https://aur.archlinux.org/packages/tardigrade)** — Unofficial AUR package for [tardigrade](https://github.com/smoothyy3/tardigrade), the self-healing terminal creature

### Experiments & Personal

- 🪦 **[github-graveyard](https://github.com/horizzon3507/github-graveyard)** — Finds abandoned open-source projects worth reviving
- 📝 **[HoryNotes](https://github.com/horizzon3507/HoryNotes)** — Floating ✦ quick-note bubble for Linux: local-first, PyQt6
- 🏷️ **[dominômetro](https://dominios.hory.one)** — Domain price comparator for Brazil — live RDAP/DNS availability, IOF + câmbio baked in

### Desktop

- 📁 **[optionFiles](https://github.com/fireflylabss/optionFiles)** — Terminal file management with as little friction as possible
- 🔎 **[optionSearch](https://github.com/fireflylabss/optionSearch)** — Instant, local-first Linux file search: CLI + GTK

### Deprecated

<details>
<summary>Superseded & archived (optionTerm, aire, opsh)</summary>

- ⌨️ **[optionTerm](https://github.com/fireflylabss/optionTerm)** — GTK4 terminal (superseded)
- ✍️ **[aire](https://github.com/fireflylabss/aire)** — Writing without distractions (deprecated)
- 🧭 **[opsh](https://github.com/fireflylabss/opsh)** — Small local-first shell in Rust (archived)

</details>

## Connect

[![Website](https://img.shields.io/badge/-hory.one-000000?style=flat-square&logo=vercel&logoColor=white)](https://hory.one)
[![X](https://img.shields.io/badge/-@horizzon3507-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/horizzon3507)
[![GitHub](https://img.shields.io/badge/-Follow-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/horizzon3507)
[![Fluxer](https://img.shields.io/badge/-gabriel%230001-5865F2?style=flat-square&logo=fluxer&logoColor=white)](https://fluxer.app)
[![Discord](https://img.shields.io/badge/-horizzon3507-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.com/users/1011380383801155614)

[![Aspas Labs](https://img.shields.io/badge/-Aspas_Labs-D32F2F?style=flat-square&logo=github&logoColor=white)](https://github.com/aspas-labs)
[![Firefly Labs](https://img.shields.io/badge/-Firefly_Labs-FF6B00?style=flat-square&logo=github&logoColor=white)](https://github.com/fireflylabss)
[![Leafole Labs](https://img.shields.io/badge/-Leafole_Labs-2E7D32?style=flat-square&logo=github&logoColor=white)](https://github.com/Leafole-Labs)
[![Aency](https://img.shields.io/badge/-Aency-6B4EFF?style=flat-square&logo=github&logoColor=white)](https://github.com/aencyorganization)
[![Basecase Labs](https://img.shields.io/badge/-Basecase_Labs-1565C0?style=flat-square&logo=github&logoColor=white)](https://github.com/Basecase-Labs)
[![Blink Team](https://img.shields.io/badge/-Blink_Team-E91E63?style=flat-square&logo=github&logoColor=white)](https://github.com/BlinkOSTeam)

## What I'm Doing

- **Building local-first software** — Desktops, CLIs, and apps that run on your machine
- **Agent-native workflows** — Figuring out how coding agents fit into real daily work
- **Shipping the antidote to bloat** — Less dashboards, more tools you actually open every day
- **Exploring around [aspaslabs.com](https://aspaslabs.com)** — And whatever else is brewing at Firefly / Leafole

## GitHub Activity

<div align="center">
  <table border="1" width="100%">
    <tr>
      <td align="center">
        <picture>
          <source
            media="(prefers-color-scheme: dark)"
            srcset="https://raw.githubusercontent.com/horizzon3507/horizzon3507/output/github-contribution-grid-snake-dark.svg"
          />
          <source
            media="(prefers-color-scheme: light)"
            srcset="https://raw.githubusercontent.com/horizzon3507/horizzon3507/output/github-contribution-grid-snake.svg"
          />
          <img
            alt="GitHub contribution snake animation"
            src="https://raw.githubusercontent.com/horizzon3507/horizzon3507/output/github-contribution-grid-snake.svg"
          />
        </picture>
      </td>
    </tr>
  </table>
</div>
