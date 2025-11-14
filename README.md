# DiaryBeast Landing Page

A minimalist landing page for DiaryBeast — a Web3 diary with gamification, built on Sui blockchain with decentralized storage and encryption.

## Overview

DiaryBeast Landing Page showcases the core features and technology stack of DiaryBeast v2, a privacy-first journaling application that combines mental health tracking, blockchain rewards, and gamification.

## Tech Stack

### Frontend Framework
- **Vite** — Fast dev server and build tool
- **React 19** + **TypeScript** — Modern UI framework
- **Tailwind CSS v3** — Utility-first CSS framework
- **Framer Motion** — Animation library for smooth interactions

### DiaryBeast v2 Technologies

The landing page reflects the technology stack used in the main DiaryBeast application:

#### Blockchain & Storage

- **[Sui Blockchain](https://sui.io)** — DIARY tokens and transactions
  - Soul-bound tokens for rewards and achievements
  - Sponsored transactions (users don't pay gas fees)
  - Move smart contracts for token economy
  - High throughput and low latency

- **[Walrus](https://www.walrus.xyz)** — Decentralized storage for diary entries
  - Encrypted entry storage on decentralized infrastructure
  - Content-addressed storage with on-chain verification
  - Cost-effective (~$0.10/GB)
  - Integration with Sui ecosystem

- **[Seal](https://seal-docs.wal.app)** — Threshold-based encryption for maximum privacy
  - Optional threshold-based encryption
  - Only the user can decrypt their entries
  - Enhanced privacy option (user choice)
  - Distributed key servers

#### Music & AI

- **[Mubert](https://mubert.com)** — AI-generated music for journaling
  - Ambient background music
  - Real-time AI music generation
  - Integrated music player in the app

### Tech Stack Icons

Technology icons are displayed in the Hero section with:
- Responsive sizing (w-8 h-8 on mobile, w-10 h-10 on desktop)
- Hover effects with colored drop shadows
- Special styling for Walrus (white background with backdrop blur)
- Text labels hidden on small screens (responsive design)
- Bullet separators between icons

## Development

### Prerequisites

- Node.js 18+ and npm

### Installation

```bash
# Install dependencies
npm install

# Start dev server (http://localhost:5173)
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Deployment

### Option 1: Via GitHub

1. Push code to GitHub repository
2. Import project in Vercel: https://vercel.com/new
3. Vercel will automatically detect Vite configuration
4. Deploy!

### Option 2: Via Vercel CLI

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel

# Production deploy
vercel --prod
```

## Project Structure

```
src/
├── components/
│   ├── Hero.tsx              # Main hero section with Beast and tech stack icons
│   ├── ConnectionSection.tsx # "You write → Beast grows" evolution timeline
│   ├── Features.tsx          # Features section (AI, Privacy, Gamification)
│   ├── Footer.tsx            # Footer with links and Sui logo
│   └── AsciiPet.tsx          # ASCII pet animations component
├── lib/
│   ├── ascii/                # ASCII animations (cat/dog states)
│   └── utils.ts              # Utility functions (cn helper)
├── App.tsx                   # Main app component
└── index.css                 # Global styles + Tailwind (Dark LCD theme)

public/
└── assets/
    ├── sui-logo.svg          # Sui blockchain logo
    ├── walrus_logo.svg       # Walrus storage logo
    ├── seal_logo.png         # Seal encryption logo
    ├── mubert.png            # Mubert music logo
    ├── diary-beast-logo-mono.svg
    ├── diary-beast-logo-colored.svg
    └── ...                   # Other assets (icons, logos)
```

## Features

- ✅ Animated ASCII Beast (breathing, reactions, state changes)
- ✅ Interactive pet states carousel (idle, happy, sad, critical, playing, eating)
- ✅ Scroll reveal animations
- ✅ Fully responsive design
- ✅ Dark LCD theme (#0A0E1A background) — matches main application
- ✅ Tech stack icons with hover effects
- ✅ Evolution timeline section
- ✅ Features showcase section
- ✅ Production-ready build

## Design

The landing page follows a minimalist design philosophy:
- **One-screen understanding** — Core value proposition visible immediately
- **Show, don't tell** — Visual demonstrations over text explanations
- **Dark LCD aesthetic** — Retro-futuristic theme matching the app

### Color Palette

- **Background**: `#0A0E1A` (Dark LCD theme)
- **Text Primary**: `#FFFFFF`
- **Text Secondary**: `#A0D8E0`
- **Accent (Beast Green)**: `#39FF14`
- **Primary (Cyan)**: `#00E5FF`
- **CTA (Blue)**: `#0052FF`
- **Success**: `#39FF14`
- **Warning**: `#FF6B00`
- **Error**: `#FF1744`
- **Tokens**: `#FFD700`

## Components

### Hero
Main landing section featuring:
- Brand logo and name
- Tagline: "What if your mental health had a face?"
- Animated ASCII Beast with state carousel
- Pet stats (HP, Joy, Tokens)
- Tech stack icons
- Launch app CTA

### Features
Showcases three core features:
- AI Progress Analysis
- Decentralized Privacy (Seal + Walrus)
- Gamified Routine

### Connection Section
Evolution timeline showing:
- Day 1: First entry
- Day 7: Building consistency
- Day 30+: Legendary status

### Footer
Footer with:
- Brand name
- Social links (Twitter, Discord, Docs)
- Technology attribution (Built on Sui)
- Legal links (Privacy, Terms)

## Related Projects

- **Main Application**: [diarybeast_v2](../diarybeast_v2) — Full DiaryBeast application
- **Documentation**: See main app's `/docs` folder for detailed technical documentation

## License

Private project — All rights reserved
