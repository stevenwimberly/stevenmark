# stevenmark2.github.io

Personal portfolio site for Steven Wimberly, ECE student at UT Austin.


## About

Portfolio documenting hardware engineering work — PCB design, embedded systems, and research. Built from scratch in HTML/CSS/JS.

---

## Structure

```
stevenmark2.github.io/
├── index.html              ← entire site, single file
├── images/
│   ├── steven.png          ← profile photo
│   └── poster.png          ← research poster preview
├── Wimberly_Symposium_Poster.pdf
└── 2025_Steven_Resume.pdf
```

---

## Sections

**Hero** — name, photo, about bio, experience, and tools in a two-column layout with an animated PCB circuit graphic as background

**Research** — SOT magnetic device work at MIT PSFC. Includes research writeup, stat cards, techniques used, and link to symposium poster PDF

**Projects** — documented PCB projects with schematic → layout → 3D model → photo carousel. Currently includes LED Strip Controller, EGSE Board, and Flight Prep Panel

**Skills** — PCB design, embedded systems, power electronics, research techniques

---

## Features

- Animated PCB trace drawing on load with signal pulse animations
- Scroll progress bar
- Bidirectional scroll reveals (elements animate in and out)
- Active nav section highlighting
- Peek carousel on project cards — schematic, layout, 3D model, photo
- Research stat blur-in animation
- Page entrance curtain fade
- Section number pulse on scroll
- Fully responsive down to mobile
- Keyboard arrow navigation on carousels
- Touch swipe support

---

## Stack

Pure HTML, CSS, and JavaScript — no build tools, no frameworks, no dependencies. Fonts loaded from Google Fonts. Hosted on GitHub Pages.

---

## Running Locally

```bash
git clone https://github.com/stevenmark2/stevenmark2.github.io
cd stevenmark2.github.io

# Any local server works — Python is simplest
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

Opening `index.html` directly in a browser also works — no server required.

---

## Adding a Project

Each project card lives in `index.html` inside `<section id="projects">`. To add a new card, duplicate an existing `.proj-card` block and update:

1. `.proj-num` — sequential number
2. `.proj-name` — project title
3. `.proj-badges` — tech stack tags
4. `.proj-status` — `s-done`, `s-wip`, or `s-plan`
5. `.whr-p` text — What / How / Results
6. Carousel slides — replace `.c-placeholder` divs with `<img src="images/your-image.png"/>`

---

## Related

- [GitHub Profile](https://github.com/stevenwimberly)
- [LinkedIn](https://linkedin.com/in/steven-wimberly-38854a222)
