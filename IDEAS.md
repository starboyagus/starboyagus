# Portfolio ideas: what to add after the planet

Your edge is rare: you can **design it (UX/UI certified), build it (code), and explain why it holds up (systems engineering)**. Most portfolios show one of these three. Make every section prove all three at once.

The planet hero already sets the tone: ASCII, pastel, a little bit cosmic. The ideas below lean into that **"small planet / mission control"** universe so the whole site feels like one world, not a template with a cool header.

---

## 1. Structure: the site as a solar system

| Section | Metaphor | What it shows |
|---|---|---|
| Hero | 🌍 Home planet | Who you are, in one line |
| About | 🛰️ Orbit | Your three sides: design, code, systems |
| Case studies | 🪐 Planets | 3–4 deep projects, not 12 shallow ones |
| Lab / playground | ☄️ Asteroid belt | Small experiments, ASCII toys, prototypes |
| Process | 🔭 Telescope | How you think: research → wireframe → build → measure |
| Contact | 📡 Transmission | Send a signal |

Navigation idea: a tiny ASCII orbit diagram in the corner, where each section is a dot circling the planet and the one you're on glows.

---

## 2. Hero upgrades

- **Rotating subtitle** that cycles through your three sides with a typewriter or scramble effect (GSAP ScrambleText is free now):
  `designing interfaces` → `writing the code` → `engineering the system`
- **Theme toggle as a planet switch:** pastel Earth ↔ pastel Mars ↔ moon. Same ASCII engine, different video or palette.
- **Click the planet → ripple.** Reuse the sharks' "splash" idea: a click sends a shockwave ring of glyphs across the grid.
- **Local time + weather glyph** in a corner: `buenos aires · 21:04 · ☁` *(swap in your city)*. It makes the page feel alive and tells recruiters your timezone.
- **"Currently" line:** `currently: studying distributed systems · building X · listening to Y`. Keep it in a JSON file so it's easy to update.

---

## 3. About: "three lenses" instead of a bio paragraph

Three cards that flip or tab between the same story told three ways:

- **👁 Designer lens:** your UX/UI certificate, a mini moodboard, and the principles you care about (accessibility, motion with purpose, clarity).
- **⌨ Developer lens:** stack as an ASCII "terminal" (`$ whoami`, `$ cat stack.txt`) that people can actually type into.
- **⚙ Engineer lens:** a systems diagram of *you*: inputs (curiosity, coffee), processes (design, build, test), outputs (products). Nerdy, memorable, and it shows you think in systems.

---

## 4. Case studies: the core of the portfolio

Pick **3–4 projects** and give each one a real case study. Use a format that shows all three skills:

1. **Problem:** who hurts and why (UX research, user quotes, metrics)
2. **Design:** wireframes → hi-fi, with the *rejected* versions and why they lost
3. **Build:** architecture diagram, key technical decisions, one interesting code snippet
4. **System view:** scalability, data flow, failure modes, trade-offs (this is where the engineering student shines)
5. **Outcome:** numbers, lessons, what you'd do differently

**Creative touches:**
- A **before/after slider** on redesigns.
- An **interactive architecture diagram**: hover a node (DB, API, cache) to see what it does and why you chose it.
- Each project gets its **own ASCII planet color** and the case study page "lands" on that planet (page-transition idea using Astro View Transitions).

**Project ideas if you need more pieces:**
- **A design system from scratch:** tokens, components, docs site. Shows UX + code + systems thinking in one artifact.
- **A redesign of your university's student portal** (unsolicited redesigns are classics because they work): research with real classmates, prototype, then build a working front-end.
- **A real-time dashboard** (monitoring a server, a game, public transit data). Shows backend, data, and good UI under pressure.
- **An accessibility audit + fix** of an open-source app, submitted as a real PR. Proof you can ship.

---

## 5. Lab / playground: the fun stuff

Small experiments, one card each, quick to make, great for social media:

- **ASCII everything:** your webcam as ASCII (pastel mode), ASCII sound visualizer, ASCII weather map.
- **Micro-interaction gallery:** buttons, toggles and loaders you designed + coded, each with a "view code" toggle.
- **Algorithms, visualized:** pathfinding, sorting, or a scheduler/OS-concept simulator (round-robin, deadlock) with a pretty UI. Bridges your engineering coursework and your design skills, and it's great for recruiters at tech companies.
- **"Break my UI":** a page with intentionally bad UX patterns and a toggle that fixes each one with an explanation. Funny, educational, and very shareable.

---

## 6. Process section: show *how* you think

- A horizontal **scroll-driven timeline** (GSAP ScrollTrigger): Discover → Define → Design → Develop → Deploy → Measure. Each step pins and shows a real artifact from your work (sticky notes, Figma frame, PR, Grafana graph).
- A **"my toolbox"** grid: Figma, VS Code, Git, Docker, Linux, whatever is actually yours, grouped by phase rather than as a logo wall.

---

## 7. Proof and credibility

- **Certificate card:** your UX/UI certificate with issuer, date and verification link, styled like a little "badge" or mission patch.
- **GitHub activity** rendered as an ASCII contribution graph (fetched at build time, so it stays static and fast).
- **Testimonials** from classmates, clients or teammates, shown as "transmissions received."
- **Uni progress bar:** `systems engineering ▓▓▓▓▓▓▓▓░░ 80%`. Honest and charming.
- **Downloadable CV** in two flavors: designer-focused and engineer-focused.

---

## 8. Writing / notes

A small blog (Astro is perfect for Markdown):

- "What a UX course didn't teach me about building real products"
- "How I made an ASCII planet from a video" (write-up of this hero)
- "Systems thinking for UI designers"
- Short TIL notes from university subjects (networks, OS, databases), explained visually.

Writing shows communication skills, which is what hiring managers search for between the lines.

---

## 9. Contact: "send a transmission"

- A form styled as a radio console: the message "encodes" into ASCII/morse before sending.
- An easter egg: type `ping` anywhere on the site → `pong 🛰️ 32ms` toast.
- Links: email, LinkedIn, GitHub, Behance/Dribbble (designers check these!), CV.

---

## 10. Easter eggs & delight (pick one or two, don't overdo it)

- **Konami code** → the planet turns into the shark ocean 🦈 (you already have the engine!).
- **Console message** for devs who open DevTools: an ASCII planet + "hey, you inspect things. we'd get along → agussv360@gmail.com".
- **`/404` page:** "lost in space": the planet floats away, with a button to get back to orbit.
- **Night mode** after 22:00 local time: the palette shifts to a moonlit lilac.

---

## 11. Technical polish (the engineer in you will like these)

- **Lighthouse 100s** across the board, with a badge in the footer that links to the report. Proof, not a claim.
- **Compress `planet.mp4`** (480p, ~500 KB) or pre-bake the ASCII frames to a small JSON. Mention it in a case study.
- **Astro View Transitions** between pages, so planets morph into each other.
- **Accessibility:** reduced-motion support (already done ✓), keyboard navigation, alt text, contrast checks on the pastel palette.
- **Open Graph image** generated at build time: your name over an ASCII planet frame for nice link previews.
- **Analytics without cookies** (Plausible / Umami) so you can show real visitor numbers in a case study about the portfolio itself.
- **Open-source the site** with a clean README. The portfolio itself becomes a portfolio piece.

---

## Suggested order

1. Compress the video + About "three lenses" section
2. Two solid case studies (one design-heavy, one systems-heavy)
3. Contact + CV
4. Lab with 2–3 experiments
5. Blog, easter eggs, polish
