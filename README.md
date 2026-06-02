# X-Template V.0.0.0-Genesis

> Cyberpunk Glassmorphism starter template — React + TypeScript + Vite

[![Deploy to GitHub Pages](https://github.com/Ex2-Axon/x-template/actions/workflows/deploy.yml/badge.svg)](https://github.com/Ex2-Axon/x-template/actions/workflows/deploy.yml)
[![Bluesky](https://img.shields.io/badge/Bluesky-%40microtronic.bsky.social-0085ff?logo=bluesky&logoColor=white)](https://bsky.app/profile/microtronic.bsky.social)

**Live demo:** https://ex2-axon.github.io/x-template/

![Screenshot](screenshot.png)

---

## Stack

| | |
|---|---|
| **Framework** | React 19 + TypeScript |
| **Build tool** | Vite 8 |
| **Styling** | CSS (Glassmorphism + Neon) + Tailwind CSS 4 |
| **Package manager** | pnpm |
| **Deploy** | GitHub Pages (auto on push) |

---

## Features

- Cyberpunk glassmorphism UI with full animation
- Neon glow effects — cyan, pink, purple, green
- Animated grid background + floating particles
- Glitch text effect on title
- Scanline CRT overlay
- Orbit rings on hero image
- Staggered entrance animations
- Auto-deploy to GitHub Pages on push
- Auto-post to Discord, Bluesky, X on push

---

## Getting Started

```bash
# Install dependencies
pnpm install

# Start dev server
pnpm dev

# Build for production
pnpm build

# Preview production build
pnpm preview
```

---

## GitHub Actions Workflows

| Workflow | Trigger | Description |
|---|---|---|
| `deploy.yml` | push to main | Build & deploy to GitHub Pages |
| `discord-notify.yml` | push to main | Send release embed to Discord |
| `bluesky-notify.yml` | push to main | Post release to Bluesky |
| `x-notify.yml` | push to main | Post release to X (Twitter) |

### Required Secrets

Go to **Settings → Secrets and variables → Actions** and add:

| Secret | Description |
|---|---|
| `DISCORD_WEBHOOK_URL` | Discord webhook URL |
| `BSKY_IDENTIFIER` | Bluesky handle (e.g. `microtronic.bsky.social`) |
| `BSKY_APP_PASSWORD` | Bluesky app password |
| `X_API_KEY` | X Consumer Key |
| `X_API_SECRET` | X Consumer Secret |
| `X_ACCESS_TOKEN` | X Access Token |
| `X_ACCESS_TOKEN_SECRET` | X Access Token Secret |

---

## Project Structure

```
x-template/
├── .github/
│   └── workflows/
│       ├── deploy.yml
│       ├── discord-notify.yml
│       ├── bluesky-notify.yml
│       └── x-notify.yml
├── public/
│   ├── favicon.svg
│   └── icons.svg
├── src/
│   ├── assets/
│   ├── App.tsx
│   ├── App.css
│   ├── index.css
│   └── main.tsx
├── package.json
└── vite.config.ts
```

---

## Connect

- Bluesky: [@microtronic.bsky.social](https://bsky.app/profile/microtronic.bsky.social)
- Discord: [Join server](https://discord.gg/8Zeq8VCU)
- GitHub: [Ex2-Axon](https://github.com/Ex2-Axon)

## Generation Prompt
```text
You are building a daily UI project. Below is the theme specification for today.

## Theme Context (daily-context.json)
```json
{
  "day": 49,
  "date": "2026-05-31",
  "version": "1.49.0",
  "project_name": "x-template-049",
  "theme": {
    "name": "Retro Terminal",
    "style": "retro-terminal",
    "mood": "monochrome, functional, nostalgic, command-line"
  },
  "palette": {
    "background": "#0c0c0c",
    "surface": "#111111",
    "primary": "#00ff41",
    "accent": "#00cc33",
    "text": "#00ff41",
    "muted": "#005c18"
  },
  "typography": {
    "heading": "Share Tech Mono",
    "body": "Share Tech Mono",
    "size": "medium"
  },
  "layout": {
    "structure": "centered",
    "density": "compact",
    "border_style": "1px solid green"
  },
  "animation": {
    "level": "minimal",
    "style": "cursor blink, typewriter"
  },
  "components": {
    "hero_text": "BOOT",
    "subtitle": "> system initialized. awaiting input_",
    "button_label": "EXEC_",
    "badge_text": "> STATUS: ONLINE"
  },
  "commit_message": "feat: UI Day 49 — Retro Terminal [fallback]",
  "source": "fallback",
  "selected_component": {
    "category": "Cards",
    "component": "zebra76966_rude-lizard-24.html",
    "path": "C:\\Users\\User\\Documents\\GitHub\\Axon\\x-components\\Cards\\zebra76966_rude-lizard-24.html",
    "content": "<div class=\"card\">\n\n  <button>\n    <svg fill=\"#000000\" preserveAspectRatio=\"xMidYMid\" xmlns:xlink=\"http://www.w3.org/1999/xlink\" xmlns=\"http://www.w3.org/2000/svg\" version=\"1.1\" viewBox=\"0 -28.5 256 256\"><g stroke-width=\"0\" id=\"SVGRepo_bgCarrier\"></g><g stroke-linejoin=\"round\" stroke-linecap=\"round\" id=\"SVGRepo_tracerCarrier\"></g><g id=\"SVGRepo_iconCarrier\"> <g> <path fill-rule=\"nonzero\" fill=\"#5865F2\" d=\"M216.856339,16.5966031 C200.285002,8.84328665 182.566144,3.2084988 164.041564,0 C161.766523,4.11318106 159.108624,9.64549908 157.276099,14.0464379 C137.583995,11.0849896 118.072967,11.0849896 98.7430163,14.0464379 C96.9108417,9.64549908 94.1925838,4.11318106 91.8971895,0 C73.3526068,3.2084988 55.6133949,8.86399117 39.0420583,16.6376612 C5.61752293,67.146514 -3.4433191,116.400813 1.08711069,164.955721 C23.2560196,181.510915 44.7403634,191.567697 65.8621325,198.148576 C71.0772151,190.971126 75.7283628,183.341335 79.7352139,175.300261 C72.104019,172.400575 64.7949724,168.822202 57.8887866,164.667963 C59.7209612,163.310589 61.5131304,161.891452 63.2445898,160.431257 C105.36741,180.133187 151.134928,180.133187 192.754523,160.431257 C194.506336,161.891452 196.298154,163.310589 198.110326,164.667963 C191.183787,168.842556 183.854737,172.420929 176.223542,175.320965 C180.230393,183.341335 184.861538,190.991831 190.096624,198.16893 C211.238746,191.588051 232.743023,181.531619 254.911949,164.955721 C260.227747,108.668201 245.831087,59.8662432 216.856339,16.5966031 Z M85.4738752,135.09489 C72.8290281,135.09489 62.4592217,123.290155 62.4592217,108.914901 C62.4592217,94.5396472 72.607595,82.7145587 85.4738752,82.7145587 C98.3405064,82.7145587 108.709962,94.5189427 108.488529,108.914901 C108.508531,123.290155 98.3405064,135.09489 85.4738752,135.09489 Z M170.525237,135.09489 C157.88039,135.09489 147.510584,123.290155 147.510584,108.914901 C147.510584,94.5396472 157.658606,82.7145587 170.525237,82.7145587 C183.391518,82.7145587 193.761324,94.5189427 193.539891,108.914901 C193.539891,123.290155 183.391518,135.09489 170.525237,135.09489 Z\"> </path> </g> </g></svg>\n  </button>\n  <button>\n    <svg xmlns=\"http://www.w3.org/2000/svg\" fill=\"none\" viewBox=\"0 0 48 48\"><g stroke-width=\"0\" id=\"SVGRepo_bgCarrier\"></g><g stroke-linejoin=\"round\" stroke-linecap=\"round\" id=\"SVGRepo_tracerCarrier\"></g><g id=\"SVGRepo_iconCarrier\"> <circle fill=\"#3B5998\" r=\"20\" cy=\"24\" cx=\"24\"></circle> <path fill=\"white\" d=\"M29.315 16.9578C28.6917 16.8331 27.8498 16.74 27.3204 16.74C25.8867 16.74 25.7936 17.3633 25.7936 18.3607V20.1361H29.3774L29.065 23.8137H25.7936V35H21.3063V23.8137H19V20.1361H21.3063V17.8613C21.3063 14.7453 22.7708 13 26.4477 13C27.7252 13 28.6602 13.187 29.8753 13.4363L29.315 16.9578Z\" clip-rule=\"evenodd\" fill-rule=\"evenodd\"></path> </g></svg>\n  </button>\n  <button>\n    <svg fill=\"#000000\" xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 1024 1024\"><g stroke-width=\"0\" id=\"SVGRepo_bgCarrier\"></g><g stroke-linejoin=\"round\" stroke-linecap=\"round\" id=\"SVGRepo_tracerCarrier\"></g><g id=\"SVGRepo_iconCarrier\"> <circle style=\"fill:#e4405f\" r=\"512\" cy=\"512\" cx=\"512\"></circle> <path style=\"fill:#fff\" d=\"M512 256c-69.5 0-78.2.3-105.5 1.5-27.3 1.3-45.8 5.6-62.1 11.9-16.8 6.5-31.1 15.3-45.4 29.5s-23 28.5-29.5 45.4c-6.3 16.3-10.6 34.9-11.9 62.1-1.3 27.3-1.5 36-1.5 105.5s.3 78.2 1.5 105.5c1.3 27.2 5.6 45.8 11.9 62.1 6.5 16.8 15.3 31.1 29.5 45.4 14.2 14.2 28.5 23 45.4 29.5 16.3 6.3 34.9 10.6 62.1 11.9 27.3 1.3 36 1.5 105.5 1.5s78.2-.3 105.5-1.5c27.2-1.3 45.8-5.6 62.1-11.9 16.8-6.5 31.1-15.3 45.4-29.5 14.2-14.2 23-28.5 29.5-45.4 6.3-16.3 10.6-34.9 11.9-62.1 1.3-27.3 1.5-36 1.5-105.5s-.3-78.2-1.5-105.5c-1.3-27.2-5.6-45.8-11.9-62.1-6.5-16.8-15.3-31.1-29.5-45.4-14.2-14.2-28.5-23-45.4-29.5-16.3-6.3-34.9-10.6-62.1-11.9-27.3-1.2-36-1.5-105.5-1.5zm0 46.1c68.3 0 76.5.3 103.5 1.5 25 1.2 38.5 5.3 47.5 8.9 12 4.6 20.5 10.2 29.5 19.1 8.9 9 14.5 17.5 19.1 29.5 3.5 9 7.7 22.5 8.8 47.5 1.2 27 1.5 35.1 1.5 103.5s-.3 76.5-1.6 103.5c-1.3 25-5.5 38.5-9 47.5-4.8 12-10.2 20.5-19.2 29.5-8.9 8.9-17.6 14.5-29.4 19.1-9 3.5-22.7 7.7-47.7 8.8-27.2 1.2-35.2 1.5-103.7 1.5s-76.5-.3-103.7-1.6c-25-1.3-38.7-5.5-47.7-9-12.1-4.8-20.5-10.2-29.4-19.2-9-8.9-14.7-17.6-19.2-29.4-3.5-9-7.7-22.7-9-47.7-1-26.9-1.3-35.2-1.3-103.3 0-68.2.3-76.5 1.3-103.7 1.3-25 5.4-38.7 9-47.7 4.5-12.2 10.2-20.5 19.2-29.5 8.9-8.9 17.3-14.7 29.4-19.2 9-3.5 22.4-7.7 47.4-9 27.2-1 35.2-1.3 103.7-1.3l1 .7zm0 78.4c-72.6 0-131.5 58.9-131.5 131.5S439.4 643.5 512 643.5 643.5 584.6 643.5 512 584.6 380.5 512 380.5zm0 216.8c-47.1 0-85.3-38.2-85.3-85.3s38.2-85.3 85.3-85.3 85.3 38.2 85.3 85.3-38.2 85.3-85.3 85.3zm167.4-221.9c0 17-13.8 30.7-30.7 30.7-17 0-30.7-13.8-30.7-30.7s13.8-30.7 30.7-30.7c16.9-.1 30.7 13.7 30.7 30.7z\"></path> </g></svg>      \n  </button><button>\n    <svg xmlns=\"http://www.w3.org/2000/svg\" fill=\"none\" viewBox=\"0 0 32 32\"><g stroke-width=\"0\" id=\"SVGRepo_bgCarrier\"></g><g stroke-linejoin=\"round\" stroke-linecap=\"round\" id=\"SVGRepo_tracerCarrier\"></g><g id=\"SVGRepo_iconCarrier\"> <path fill=\"#47ACDF\" d=\"M11.7887 28C8.55374 28 5.53817 27.0591 3 25.4356C5.15499 25.5751 8.95807 25.2411 11.3236 22.9848C7.76508 22.8215 6.16026 20.0923 5.95094 18.926C6.25329 19.0426 7.6953 19.1826 8.50934 18.856C4.4159 17.8296 3.78793 14.2373 3.92748 13.141C4.695 13.6775 5.99745 13.8641 6.50913 13.8174C2.69479 11.0882 4.06703 6.98276 4.74151 6.09635C7.47882 9.88867 11.5812 12.0186 16.6564 12.137C16.5607 11.7174 16.5102 11.2804 16.5102 10.8316C16.5102 7.61092 19.1134 5 22.3247 5C24.0025 5 25.5144 5.71275 26.5757 6.85284C27.6969 6.59011 29.3843 5.97507 30.2092 5.4432C29.7934 6.93611 28.4989 8.18149 27.7159 8.64308C27.7224 8.65878 27.7095 8.62731 27.7159 8.64308C28.4037 8.53904 30.2648 8.18137 31 7.68256C30.6364 8.52125 29.264 9.91573 28.1377 10.6964C28.3473 19.9381 21.2765 28 11.7887 28Z\"></path> </g></svg>\n  </button>\n\n\n</div>\n\n<style>\n/* Tags: twitter, facebook, instagram, card, Discord, share, multicolor */\n.card {\n  width: 290px;\n  height: 64px;\n  background: rgb(255, 255, 255);\n  display: flex;\n  align-items: center;\n  justify-content: space-between;\n  padding: 10px;\n  border-radius: 20px;\n  position: relative;\n  border: 2px solid transparent;\n  transition: all 0.5s ease-in-out;\n}\n\n.card:focus-within {\n  background-color: rgba(17, 17, 17, 0.5);\n  backdrop-filter: blur(10px);\n  border: 2px solid rgb(27, 27, 27);\n  box-shadow: 0 0 10px rgba(255, 255, 255, 0.5);\n}\n\n.card button {\n  font-size: 34px;\n  background-color: transparent;\n  width: 50px;\n  padding: 7px;\n  height: 50px;\n  border-radius: 100%;\n  transition: all 0.2s ease-in;\n  border: 0;\n  cursor: pointer;\n}\n\n.card button:focus {\n  background-color: rgb(255, 255, 255);\n  margin-bottom: 50%;\n}\n\n.card::hover {\n}\n\n\n</style>"
  }
}
```

## Selected Component Reference
- Category: Cards
- Component: zebra76966_rude-lizard-24.html
- Path: C:\Users\User\Documents\GitHub\Axon\x-components\Cards\zebra76966_rude-lizard-24.html

Use the selected component HTML below as the primary design reference for the new UI. Keep the structure and styling assumptions in mind while rewriting the requested files.
```html
<div class="card">

  <button>
    <svg fill="#000000" preserveAspectRatio="xMidYMid" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns="http://www.w3.org/2000/svg" version="1.1" viewBox="0 -28.5 256 256"><g stroke-width="0" id="SVGRepo_bgCarrier"></g><g stroke-linejoin="round" stroke-linecap="round" id="SVGRepo_tracerCarrier"></g><g id="SVGRepo_iconCarrier"> <g> <path fill-rule="nonzero" fill="#5865F2" d="M216.856339,16.5966031 C200.285002,8.84328665 182.566144,3.2084988 164.041564,0 C161.766523,4.11318106 159.108624,9.64549908 157.276099,14.0464379 C137.583995,11.0849896 118.072967,11.0849896 98.7430163,14.0464379 C96.9108417,9.64549908 94.1925838,4.11318106 91.8971895,0 C73.3526068,3.2084988 55.6133949,8.86399117 39.0420583,16.6376612 C5.61752293,67.146514 -3.4433191,116.400813 1.08711069,164.955721 C23.2560196,181.510915 44.7403634,191.567697 65.8621325,198.148576 C71.0772151,190.971126 75.7283628,183.341335 79.7352139,175.300261 C72.104019,172.400575 64.7949724,168.822202 57.8887866,164.667963 C59.7209612,163.310589 61.5131304,161.891452 63.2445898,160.431257 C105.36741,180.133187 151.134928,180.133187 192.754523,160.431257 C194.506336,161.891452 196.298154,163.310589 198.110326,164.667963 C191.183787,168.842556 183.854737,172.420929 176.223542,175.320965 C180.230393,183.341335 184.861538,190.991831 190.096624,198.16893 C211.238746,191.588051 232.743023,181.531619 254.911949,164.955721 C260.227747,108.668201 245.831087,59.8662432 216.856339,16.5966031 Z M85.4738752,135.09489 C72.8290281,135.09489 62.4592217,123.290155 62.4592217,108.914901 C62.4592217,94.5396472 72.607595,82.7145587 85.4738752,82.7145587 C98.3405064,82.7145587 108.709962,94.5189427 108.488529,108.914901 C108.508531,123.290155 98.3405064,135.09489 85.4738752,135.09489 Z M170.525237,135.09489 C157.88039,135.09489 147.510584,123.290155 147.510584,108.914901 C147.510584,94.5396472 157.658606,82.7145587 170.525237,82.7145587 C183.391518,82.7145587 193.761324,94.5189427 193.539891,108.914901 C193.539891,123.290155 183.391518,135.09489 170.525237,135.09489 Z"> </path> </g> </g></svg>
  </button>
  <button>
    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 48 48"><g stroke-width="0" id="SVGRepo_bgCarrier"></g><g stroke-linejoin="round" stroke-linecap="round" id="SVGRepo_tracerCarrier"></g><g id="SVGRepo_iconCarrier"> <circle fill="#3B5998" r="20" cy="24" cx="24"></circle> <path fill="white" d="M29.315 16.9578C28.6917 16.8331 27.8498 16.74 27.3204 16.74C25.8867 16.74 25.7936 17.3633 25.7936 18.3607V20.1361H29.3774L29.065 23.8137H25.7936V35H21.3063V23.8137H19V20.1361H21.3063V17.8613C21.3063 14.7453 22.7708 13 26.4477 13C27.7252 13 28.6602 13.187 29.8753 13.4363L29.315 16.9578Z" clip-rule="evenodd" fill-rule="evenodd"></path> </g></svg>
  </button>
  <button>
    <svg fill="#000000" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1024 1024"><g stroke-width="0" id="SVGRepo_bgCarrier"></g><g stroke-linejoin="round" stroke-linecap="round" id="SVGRepo_tracerCarrier"></g><g id="SVGRepo_iconCarrier"> <circle style="fill:#e4405f" r="512" cy="512" cx="512"></circle> <path style="fill:#fff" d="M512 256c-69.5 0-78.2.3-105.5 1.5-27.3 1.3-45.8 5.6-62.1 11.9-16.8 6.5-31.1 15.3-45.4 29.5s-23 28.5-29.5 45.4c-6.3 16.3-10.6 34.9-11.9 62.1-1.3 27.3-1.5 36-1.5 105.5s.3 78.2 1.5 105.5c1.3 27.2 5.6 45.8 11.9 62.1 6.5 16.8 15.3 31.1 29.5 45.4 14.2 14.2 28.5 23 45.4 29.5 16.3 6.3 34.9 10.6 62.1 11.9 27.3 1.3 36 1.5 105.5 1.5s78.2-.3 105.5-1.5c27.2-1.3 45.8-5.6 62.1-11.9 16.8-6.5 31.1-15.3 45.4-29.5 14.2-14.2 23-28.5 29.5-45.4 6.3-16.3 10.6-34.9 11.9-62.1 1.3-27.3 1.5-36 1.5-105.5s-.3-78.2-1.5-105.5c-1.3-27.2-5.6-45.8-11.9-62.1-6.5-16.8-15.3-31.1-29.5-45.4-14.2-14.2-28.5-23-45.4-29.5-16.3-6.3-34.9-10.6-62.1-11.9-27.3-1.2-36-1.5-105.5-1.5zm0 46.1c68.3 0 76.5.3 103.5 1.5 25 1.2 38.5 5.3 47.5 8.9 12 4.6 20.5 10.2 29.5 19.1 8.9 9 14.5 17.5 19.1 29.5 3.5 9 7.7 22.5 8.8 47.5 1.2 27 1.5 35.1 1.5 103.5s-.3 76.5-1.6 103.5c-1.3 25-5.5 38.5-9 47.5-4.8 12-10.2 20.5-19.2 29.5-8.9 8.9-17.6 14.5-29.4 19.1-9 3.5-22.7 7.7-47.7 8.8-27.2 1.2-35.2 1.5-103.7 1.5s-76.5-.3-103.7-1.6c-25-1.3-38.7-5.5-47.7-9-12.1-4.8-20.5-10.2-29.4-19.2-9-8.9-14.7-17.6-19.2-29.4-3.5-9-7.7-22.7-9-47.7-1-26.9-1.3-35.2-1.3-103.3 0-68.2.3-76.5 1.3-103.7 1.3-25 5.4-38.7 9-47.7 4.5-12.2 10.2-20.5 19.2-29.5 8.9-8.9 17.3-14.7 29.4-19.2 9-3.5 22.4-7.7 47.4-9 27.2-1 35.2-1.3 103.7-1.3l1 .7zm0 78.4c-72.6 0-131.5 58.9-131.5 131.5S439.4 643.5 512 643.5 643.5 584.6 643.5 512 584.6 380.5 512 380.5zm0 216.8c-47.1 0-85.3-38.2-85.3-85.3s38.2-85.3 85.3-85.3 85.3 38.2 85.3 85.3-38.2 85.3-85.3 85.3zm167.4-221.9c0 17-13.8 30.7-30.7 30.7-17 0-30.7-13.8-30.7-30.7s13.8-30.7 30.7-30.7c16.9-.1 30.7 13.7 30.7 30.7z"></path> </g></svg>      
  </button><button>
    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 32 32"><g stroke-width="0" id="SVGRepo_bgCarrier"></g><g stroke-linejoin="round" stroke-linecap="round" id="SVGRepo_tracerCarrier"></g><g id="SVGRepo_iconCarrier"> <path fill="#47ACDF" d="M11.7887 28C8.55374 28 5.53817 27.0591 3 25.4356C5.15499 25.5751 8.95807 25.2411 11.3236 22.9848C7.76508 22.8215 6.16026 20.0923 5.95094 18.926C6.25329 19.0426 7.6953 19.1826 8.50934 18.856C4.4159 17.8296 3.78793 14.2373 3.92748 13.141C4.695 13.6775 5.99745 13.8641 6.50913 13.8174C2.69479 11.0882 4.06703 6.98276 4.74151 6.09635C7.47882 9.88867 11.5812 12.0186 16.6564 12.137C16.5607 11.7174 16.5102 11.2804 16.5102 10.8316C16.5102 7.61092 19.1134 5 22.3247 5C24.0025 5 25.5144 5.71275 26.5757 6.85284C27.6969 6.59011 29.3843 5.97507 30.2092 5.4432C29.7934 6.93611 28.4989 8.18149 27.7159 8.64308C27.7224 8.65878 27.7095 8.62731 27.7159 8.64308C28.4037 8.53904 30.2648 8.18137 31 7.68256C30.6364 8.52125 29.264 9.91573 28.1377 10.6964C28.3473 19.9381 21.2765 28 11.7887 28Z"></path> </g></svg>
  </button>


</div>

<style>
/* Tags: twitter, facebook, instagram, card, Discord, share, multicolor */
.card {
  width: 290px;
  height: 64px;
  background: rgb(255, 255, 255);
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 10px;
  border-radius: 20px;
  position: relative;
  border: 2px solid transparent;
  transition: all 0.5s ease-in-out;
}

.card:focus-within {
  background-color: rgba(17, 17, 17, 0.5);
  backdrop-filter: blur(10px);
  border: 2px solid rgb(27, 27, 27);
  box-shadow: 0 0 10px rgba(255, 255, 255, 0.5);
}

.card button {
  font-size: 34px;
  background-color: transparent;
  width: 50px;
  padding: 7px;
  height: 50px;
  border-radius: 100%;
  transition: all 0.2s ease-in;
  border: 0;
  cursor: pointer;
}

.card button:focus {
  background-color: rgb(255, 255, 255);
  margin-bottom: 50%;
}

.card::hover {
}


</style>
```

## Your Task
Completely redesign the UI by rewriting these three files from scratch:
- `src/App.tsx`
- `src/App.css`
- `src/index.css`

## Rules for App.tsx
1. Keep ALL existing imports:
   - `import { useState, useEffect, useRef } from 'react'`
   - `import reactLogo from './assets/react.svg'`
   - `import viteLogo from './assets/vite.svg'`
   - `import heroImg from './assets/hero.png'`
   - `import './App.css'`
2. Keep the `CounterNum` component (useRef + useEffect animation)
3. Keep the counter button with `onClick` / `setCount` handler
4. Keep the Documentation section (Vite/React links)
5. Keep the Social section (GitHub/Discord/X/Bluesky links + SVG icons)
6. Do NOT use CSS custom properties (`--var-name`) in inline `style` attributes - TypeScript will error

## Rules for CSS
- Apply the palette, typography, layout structure, animation level, and component text from the JSON above
- Use Google Fonts via `@import` in `index.css`
- Match the theme mood: monochrome, functional, nostalgic, command-line

## Mandatory Requirements (apply to every build)

### 1. Responsive - Mobile First
- Design for mobile (320px) first, scale up with `min-width` breakpoints
- Touch targets minimum 44x44px
- No horizontal scroll on any screen size
- Fluid typography: use `clamp()` or responsive units (`rem`, `%`, `vw`)
- Images and layout must reflow gracefully at 320px, 768px, 1280px

### 2. Footer Copyright
- The page MUST have a `<footer>` at the bottom
- Footer text: `© 2026 Microtronic Co., Ltd. All rights reserved. Credit By Axon.`
- Legal: [Privacy Policy](https://microtronic-thailand.github.io/privacy-policy/?lang=en)
- Style the footer to match the theme palette (muted text on surface background)

### 3. SEO Standards
- `index.html` must have a descriptive `<title>`: `BOOT - Retro Terminal | Microtronic`
- Add `<meta name="description">` with the subtitle: `> system initialized. awaiting input_`
- Add `<meta name="keywords">` relevant to the theme
- Add Open Graph tags: `og:title`, `og:description`, `og:type` (website)
- All images must have meaningful `alt` attributes
- Use semantic HTML: `<header>`, `<main>`, `<section>`, `<footer>`, `<nav>` where appropriate
- Heading hierarchy: one `<h1>` (hero), `<h2>` for sections - no skipping levels

### 4. Extreme Effects & Animations
- Add extremely impressive effects and animations (multiply by 10) to make it look stunning!
- Focus on hover effects, background animations, micro-interactions, and parallax.

## After saving all files
1. Update `version` in `package.json` to `1.49.0`
2. Update `<title>` and meta tags in `index.html` as specified above
3. Run: `pnpm build`
4. If build succeeds → write `done` to `scripts/build-done.flag`
5. If build fails with TypeScript errors → fix them and rebuild

```
