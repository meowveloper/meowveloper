# Zwe Khant Aung (meowveloper)
> TypeScript, Zig, Nix, Linux<br/>
> Full Stack Developer & Systems Enthusiast<br/>
> Bangkok, Thailand | +66822918935 | meowveloper.dev@gmail.com<br/>
> Github: [meowveloper](https://github.com/meowveloper)<br/>
> Education: Bachelor of Computer Science, University of Sunderland (UK)

## About Me
<div style="text-align: justify;">
Full Stack Engineer with a Systems Mindset I build high-level web applications with <strong>NuxtJS</strong>, <strong>React</strong> and <strong>TypeScript</strong>, while exploring low-level performance with Zig. Whether I'm optimizing SEO for an EdTech marketplace or managing memory in a custom CLI tool, my goal is always the same: speed, type-safety, and reproducibility. Even though I am currently focusing on improving my system programming knowledge, I can also handle wherever the typescript touches.
</div>
<br/>

## Professional Experience
### Frontend Engineer | September 2024 – April 2026 ([Arsari](https://arsari.app))
Developed and architected the frontend of Arsari, a comprehensive educator-learner platform, using Nuxt.js, Vue 3, and TypeScript. Spearheaded the transition from a basic landing page to a complex, real-time education ecosystem.
- Real-time Communication: Built a robust chat system and live support feature using Laravel Echo and Pusher, implementing real-time online status tracking, heartbeat mechanisms, and automated message grouping.
- Complex State Management: Engineered a sophisticated educator profile management system with a draft-save mechanism, shared state between view/edit modes, and dynamic data caching using Nuxt middleware.
- Onboarding & UI/UX: Designed and implemented a multi-step educator onboarding process featuring a real-time profile completion progress bar and complex class creation forms.
- Scheduling Systems: Integrated and customized FullCalendar to handle educator availability, featuring complex UTC-to-local timezone synchronization and dynamic time-slot management.
- Search & SEO Optimization: Developed SEO-friendly dynamic routing for course discovery and integrated metadata management, significantly enhancing the platform's visibility for educators and courses.
- Analytics & Monitoring: Led the integration of a full observability and marketing suite, including Sentry for error tracking, Posthog for product analytics, Meta Pixel, and Google Analytics (Gtag).
- Internationalization (i18n): Managed full localization for English and Burmese (MM) markets, including specialized currency formatting, locale-aware category filtering, and RTL-compatible UI adjustments.
- Security & Authentication: Implemented secure OTP (One-Time Password) authentication flows and integrated Social Auth (Google/Facebook) while maintaining strict environment variable security.
- DevOps & Tooling: Established consistent development environments using Docker Dev Containers and optimized build processes by migrating credentials to server-side runtime configurations.
- Official website link: [https://arsari.app](https://arsari.app)
<br/>
<div style="page-break-after: always;"></div>

## Projects
### Password Strength Auditor [(psa)](https://github.com/meowveloper/psa.git)
- PSA is a high-performance, cross-platform command-line tool designed for auditing password strength. Written in Zig(0.15.2), it leverages **manual memory management** and **zero-allocation optimization** to deliver maximum speed.
- Features:
    - **Dictionary** Attack: High-speed wordlist checking with optimized file I/O.
    - **Brute-Force** Attack: Recursive character combination generation with interactive configuration.
    - Audit Mode: Batch processing of multiple hashes with automated security scoring and reporting.
    - **Cross-Platform**: Compiles natively for Linux, Windows, and macOS.
    - Zero Dependencies: Uses Zig's standard library for all cryptography (MD5) and I/O.
- github link: [https://github.com/meowveloper/psa.git](https://github.com/meowveloper/psa.git)
### meowmux [(meowmux)](https://github.com/meowveloper/meowmux.git)
- Meowmux is a lightweight, TUI-based CLI project manager written in Zig (0.15.2). It simplifies workflow by allowing you to quickly manage and switch between projects, automatically launching them in tmux sessions.
- Features:
    - Interactive **TUI**: Navigate your project list with ease using **Vim-style** keys (j/k) or arrow keys implemented with **self-written** terminal cleaning and UI logic **without any external libraries**.
    - Project Management: Add, Edit, and Delete projects directly from the interface.
    - Tmux Integration: **Automatically creates or attaches** to a named tmux session for the selected project.
    - Path Autocomplete: Supports tab-completion for file paths when adding or editing projects with **self-written** file system iterating and search logic **without any external libraries**.
    - Config persistence: Safely stores your project list in `~/.config/meowmux/projects.json`.
- github link: [https://github.com/meowveloper/meowmux.git](https://github.com/meowveloper/meowmux.git)
### meowkey [(meowkey)](https://github.com/meowveloper/meowkey.git)
- Meowkey is a lightweight background process for Linux, written in **Zig**, designed to generate mechanical keyboard sounds in real-time as you type.
- Core Objectives:
    - **Zero Latency:** Minimize the delay between physical key presses and audio feedback.
    - **Global Input Capture:** Utilize the Linux Input Subsystem (`/dev/input/event*`) to intercept keystrokes regardless of which window is active.
    - **Low Resource Usage:** Leverage Zig's efficiency to ensure the process remains unnoticeable in the background.
    - **ALSA Integration:** Direct interfacing with the Advanced Linux Sound Architecture for high-performance audio playback.
- Technical Architecture:
    1. **Input Listener**: The application will read from one or more `/dev/input/event*` devices. It filters for `EV_KEY` events to detect `KEY_DOWN` transitions.
    2. **Audio Engine**: A low-latency buffer management system using ALSA.
- github link: [https://github.com/meowveloper/meowkey.git](https://github.com/meowveloper/meowkey.git)
## DevOps & Developer Experience
* **Reproducible Environments:** Expert in **Nix/NixOS** (daily driver) and **Flakes** for creating zero-latency development shells (`nix develop`).
* **Environment Parity:** Replaced bloated Docker-based local workflows with native, deterministic Nix environments, reducing build times by 30% and local resource overhead.
* **Infrastructure as Code:** Declaratively manage system-wide configurations, ensuring consistent setups across multiple machines.
