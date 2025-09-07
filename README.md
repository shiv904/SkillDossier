# SkillDossier

A modern, responsive mentorship platform frontend built with Vite, React, TailwindCSS, and Framer Motion.

## Tech Stack
- Vite + React
- TailwindCSS (dark mode via class)
- Framer Motion (animations)
- React Router (routing)

## Features
- Clean, professional UI/UX with semantic HTML and a11y
- Navbar with dark/light toggle and responsive menu
- Pages: Home, Mentors (dynamic grid), Dashboard, Contact, Register
- Forms with client-side validation (required, email)
- Smooth animations and page transitions
- Mock API: fetches mentors from `/mentors.json`
- Fully responsive (mobile/tablet/desktop)

## Project Structure
```
src/
  components/ (Navbar, Footer, MentorCard, Forms)
  pages/ (Home.jsx, Mentors.jsx, Dashboard.jsx, Contact.jsx)
  sections/ (Hero.jsx)
  App.jsx, main.jsx, index.css
public/
  mentors.json
```

## Setup
```bash
npm install
npm run dev
```
- App runs on `http://localhost:5173` (default Vite port).

## Build
```bash
npm run build
npm run preview
```
- Build output in `dist/` (ready for deployment).

## Deployment
- GitHub
  - git init && git add . && git commit -m "feat: initial"
  - Create repo: `skilldossier` → add remote and push
  - git remote add origin https://github.com/<your-username>/skilldossier.git
  - git branch -M main && git push -u origin main

- Netlify (recommended)
  - Connect repo → Build command: `npm run build` → Publish directory: `dist`
  - SPA routing: ensured via `public/_redirects` → `/* /index.html 200`
  - Live URL: https://<your-site>.netlify.app

- Vercel
  - Import repo → Framework preset: Vite
  - Build command `npm run build`, Output `dist`
  - Live URL: https://<your-project>.vercel.app

## Screenshots
- Add screenshots to `docs/` and reference here.

## Accessibility Notes
- Semantic regions: `header`, `nav`, `main`, `footer`
- ARIA labels on interactive icons/buttons
- Visible focus styles and keyboard-friendly navigation
- Alt text for all images

## License
MIT

