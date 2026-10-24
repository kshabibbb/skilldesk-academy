# SkillDesk Academy — IT Support Learning Website

A fully functional, free self-study website for learning IT support from scratch.

## What is included

- **8 courses, 36 real lessons**, beginner through early intermediate
- **72 knowledge-check questions** with explanations, retakes, and progress tracking
- **Hands-on checklists** attached to every lesson
- **8 interactive help-desk cases** for diagnostic decision-making
- **Simulated terminal** (examples only: no real system or network operations)
- **36-term IT glossary**, quick-reference toolkit, and copyable ticket template
- **Private, browser-local saved progress and notes**, with JSON export/import
- Responsive desktop and mobile interface; no external dependencies or accounts

## Open the website

1. Unzip the archive.
2. Open `index.html` in a modern browser (Chrome, Edge, Firefox, Safari).
3. Choose **IT Support Foundations**, then work through the lessons and quizzes.

For a single-file version that needs no accompanying files, open the separate `SkillDesk_Academy_Offline.html` downloadable from ChatGPT. All functionality works without an internet connection.

## Customize or publish

- `index.html` — base page
- `styles.css` — responsive visual styling
- `data.js` — course content and learning scenarios (edit this to add lessons)
- `app.js` — routing, navigation, quizzes, practice tools, and saved progress

To make this a public website, upload these **four files together** to a static hosting platform such as GitHub Pages, Netlify, or Cloudflare Pages. `index.html` should be the main entry point. No server, database, or build process is required.

## Important details

- No sign-in is required. Saved progress is specific to your current browser/device and can be lost if browser site data is cleared or private browsing ends. Use **Toolkit → Export progress** for a backup; the same section can import it.
- The terminal is **not** a real shell. Its examples use simulated diagnostic responses, including reserved sample addresses.
- Practice cases and tickets are fictional. Never run invasive scans or make changes to a school/employer network without permission.
- This is an independent educational resource, not a CompTIA or other official certification or accredited program.

© 2026 SkillDesk Academy — educational demo website.


## Updating the existing Cloudflare Worker
1. Go to Cloudflare Dashboard → Workers & Pages → `skilldesk-academy`.
2. Select **New deployment** and use the static assets upload option.
3. Upload the ZIP in this package (or all five root files) and deploy to the existing Worker. Do not create a new project.
4. Check `https://skilldesk-academy.skilldesk.workers.dev/#/about`.

The About page was added without changing local storage keys, so current progress should remain available in the same browser and origin. Always export progress from **My learning** before substantial future changes.
