# Lamla Quiz Hub

A single platform for KNUST Computer Science Year 2 students to access multiple practice tests — built with [Astro](https://astro.build) and deployed on Netlify.

## Live site

[lamla-quiz-hub.netlify.app](https://lamla-quiz-hub.netlify.app)

## What it is

Lamla Quiz Hub is built specifically for KNUST CS Year 2 students. Past questions and course material across multiple Year 2 courses are transformed into interactive quizzes, all accessible from one place — no hunting across different files, group chats, or links.

The flow is simple: landing page → course hub → quiz page. Pick a subject, open the quiz, and start practicing immediately.

**Available courses**

| Course | Status |
|---|---|
| Literature | Live |
| Operating Systems | Live |
| Electronics | Organizing |
| OOP with Java | Coming soon |
| Ethical Computing | Coming soon |
| Linear & Numerical Algebra | Coming soon |
| System Analysis & Design | Coming soon |
| Database Concepts & Technologies | Coming soon |

## Project structure

```
quizzes/
├── src/
│   ├── pages/          # One .astro file per route
│   ├── components/     # Shared UI components (Navbar, etc.)
│   ├── layouts/        # Page layout wrapper
│   └── data/           # Quiz question data
├── public/             # Static assets (images, favicon)
├── astro.config.mjs
├── netlify.toml
└── package.json
```

## Local development

```bash
npm install
npm run dev
```

## Build

```bash
npm run build      # outputs to dist/
npm run preview    # preview the built site locally
```

## Deployment

The site deploys automatically via Netlify. The `netlify.toml` sets the build command and publish directory. Make sure Netlify's **base directory** is set to `quizzes` in the site settings.

## Related

[Lamla AI](https://lamla-ai.vercel.app) — the AI-powered study tool built by the developer of this hub.