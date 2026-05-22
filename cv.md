# Zwe Khant Aung (meowveloper)
> TypeScript, Zig, Nix, Linux<br/>
> Full Stack Developer & Systems Enthusiast<br/>
> Bangkok, Thailand | +66822918935 | meowveloper.dev@gmail.com<br/>
> Github: [meowveloper](https://github.com/meowveloper)<br/>
> Education: Bachelor of Computer Science, University of Sunderland (UK)<br/>
> Portfolio: [meowveloper](https://unbound-ink.vercel.app/p/meow)

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

### Lead Full-Stack Developer | [Unbound (The Independent Ink)](https://unbound-ink.vercel.app) December 2025 – May 2026
Architected and developed Unbound, a high-performance digital publishing and professional reputation platform built with Next.js 16 (App Router), React 19, and Convex (Serverless).
- Security & Authentication: Engineered a custom authentication system from scratch using PBKDF2 password hashing and secure session management via httpOnly cookies, avoiding third-party provider dependencies.
- Reputation Engine: Developed a comprehensive "Proof of Work" ecosystem, including professional portfolios (/p/[username]) with Bento Grid layouts and a verifiable badge system linked to professional artifacts and case studies.
- Content Systems: Integrated the Tiptap rich-text editor with automated draft synchronization, supporting multi-part "Serial" stories and "Single" document formats (Articles/Manifestos) with optimized reader interfaces.
- Advanced Feed Architecture: Optimized social discovery by implementing a Global Index + Memory Filter strategy for the activity feed, enabling high-performance dual-stream merging of followed users and "Official" platform announcements.
- Monetization & Analytics: Launched "Phase 1" of a non-intrusive monetization model based on Usage Time, utilizing the Visibility API for client-side heartbeat tracking and background aggregate processing.
- System Reliability: Established a 3-tier testing infrastructure (Backend, Vitest/RTL), achieving a 100% pass rate across 140+ tests covering declarative effect systems and social graph logic.
- SEO & AISO: Implemented Artificial Intelligence Search Optimization (AISO) and structured data using JSON-LD (Schema.org), dynamic sitemaps, and semantic HTML5 to maximize discoverability for both search engines and AI agents.
- Backend Engineering: Hardened database integrity through a declarative Effect System for aggregates, robust cascading deletion background jobs, and strict Convex validator enforcement to prevent data injection.
- Administrative Tooling: Built a secure Admin Control Center featuring real-time user search, badge governance workflows (reporting/revocation), and narrative management for verified credentials.
- Official website link: [https://unbound-ink.vercel.app](https://unbound-ink.vercel.app)
- My **portfolio** on Unbound: [meowveloper](https://unbound-ink.vercel.app/p/meow)
<br/>
<div style="page-break-after: always;"></div>

## Projects
### Password Strength Auditor [(psa)](https://github.com/meowveloper/psa.git)
- PSA is a high-performance, cross-platform command-line tool designed for auditing password strength. Written in Zig(0.15.2), it leverages **manual memory management** and **zero-allocation optimization** to deliver maximum speed. **This was written for my Computer Science Bachelor Degree**
- Features:
    - **Dictionary** Attack: High-speed wordlist checking with optimized file I/O.
    - **Brute-Force** Attack: Recursive character combination generation with interactive configuration.
    - Audit Mode: Batch processing of multiple hashes with automated security scoring and reporting.
    - **Cross-Platform**: Compiles natively for Linux, Windows, and macOS.
    - Zero Dependencies: Uses Zig's standard library for all cryptography (MD5) and I/O.
- github link: [https://github.com/meowveloper/psa.git](https://github.com/meowveloper/psa.git)
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
