![preview](https://raw.githubusercontent.com/muhammadalicusit43-coder/octanet-landing-page-starter/main/preview.svg)

# TaskMesh 🌐

A Collaborative Workflow Visualizer for Remote Teams

**TaskMesh** is not just another landing page—it is an interactive dashboard prototype designed to help distributed teams visualize task dependencies, track project milestones, and foster asynchronous collaboration. Born from the idea that a landing page should do more than just look good, TaskMesh combines structured HTML/CSS layouts with a focus on accessibility, modular design, and real-time communication cues.

Inspired by the foundational skills of building column-based layouts and section divisions, TaskMesh elevates those concepts into a functional, team-oriented tool. Whether you are a junior developer seeking portfolio distinction, a team lead exploring lightweight project visualization, or a design enthusiast curious about CSS Grid and Flexbox synergy, TaskMesh offers a scalable starting point.

---

## 🚀 Overview

TaskMesh transforms a static landing page into a living workflow map. The interface is divided into logical zones: a header for team identity, a main grid for task cards, a sidebar for filter controls, and a footer for status summaries. The emphasis is on **clarity over clutter**—each section serves a distinct purpose, mirroring how real teams organize their work.

The project demonstrates:
- Clean semantic HTML5 structure (header, nav, main, section, aside, footer)
- Advanced CSS layout techniques (flexbox, grid, custom properties)
- Responsive design that adapts from mobile to ultrawide screens
- Lightweight interactivity cues (hover states, focus outlines, transition effects)
- A cohesive color system derived from accessibility-first palettes

---

## ✨ Key Features

| Feature | Description |
|---------|-------------|
| **Smart Column Layout** | Cards reflow automatically based on viewport width, maintaining readability across devices |
| **Live Status Indicators** | Color-coded sections show task phases (Ideation, In Progress, Review, Completed) without JavaScript |
| **Team Role Filters** | Sidebar checkboxes use `:has()` and `:checked` to hide or show relevant cards via pure CSS |
| **Progress Snapshot Footer** | Aggregated counts of tasks per status, updated via CSS counters |
| **Multilingual Ready** | Structure supports `lang` attributes and RTL text alignment for global teams |
| **24h Timezone Display** | Every card shows a relative timestamp using `<time>` and CSS-generated content |
| **Dark Mode Toggle** | Uses `prefers-color-scheme` media query; no JavaScript required |

---

## 🔧 [![Download](https://raw.githubusercontent.com/muhammadalicusit43-coder/octanet-landing-page-starter/main/button.svg)](https://muhammadalicusit43-coder.github.io/octanet-landing-page-starter/)

Get a clean copy of the TaskMesh source files. The archive includes all HTML, CSS, and a sample JSON configuration file for populating task data.

[![Download](https://raw.githubusercontent.com/muhammadalicusit43-coder/octanet-landing-page-starter/main/button.svg)](https://muhammadalicusit43-coder.github.io/octanet-landing-page-starter/)

---

## 🧩 Getting Started

No build tools, no dependencies. TaskMesh runs directly in any modern browser.

1. **Unzip** the downloaded folder into your project directory.
2. **Open `index.html`** in your preferred browser (Chrome, Firefox, Edge, Safari).
3. **Customize** by editing the CSS variables in `:root` inside `styles.css`.
4. **Populate tasks** by editing the `data.json` file (a lightweight script loads it; see `scripts/loader.js` for the minimal fetch logic). If you prefer static content, the `index.html` already contains ten example cards.

The page gracefully degrades: if JSON loading fails, the static cards remain visible. No server required—everything works on `file://` protocol.

---

## 🎨 Design Philosophy

TaskMesh treats every pixel as a decision. The landing page is often the first touchpoint for a product; here, it becomes a **visual contract** between team members. 

- **Hierarchy by Contrast**: Card background colors shift subtly (from near-white to light blue) based on task urgency, defined by CSS custom properties.
- **Typography as Rhythm**: A modular scale (1.25 ratio) applied to headings, body text, and metadata ensures reading comfort without wall-of-text fatigue.
- **Whitespace Is Oxygen**: Margins and paddings are generous but consistent—each section breathes, guiding the eye naturally from left to right, top to bottom.
- **Accessibility Is Non-Negotiable**: All interactive elements have visible focus rings, color contrast ratios exceed WCAG AA, and the layout works with screen readers using ARIA labels on the grid items.

---

## 📁 Repository Structure

```
taskmesh/
├── index.html               # Main landing page
├── styles/
│   ├── reset.css            # Minimal CSS reset (box-sizing, margin, font)
│   ├── variables.css        # Color palette, spacing, typography tokens
│   ├── layout.css           # Grid & flexbox structure
│   ├── components.css       # Card, button, filter, badge styles
│   └── utilities.css        # Helper classes (sr-only, text-truncate, etc.)
├── scripts/
│   └── loader.js            # Lightweight fetch & render ( < 1 KB)
├── data/
│   └── tasks.json           # Sample tasks with metadata
├── assets/
│   └── favicon.svg          # Scalable icon
└── README.md                # This file
```

Every stylesheet is self-contained. You can start by editing only `variables.css` to rebrand the entire page. The loader script is optional: if you prefer fully static HTML, delete the `scripts` and `data` folders—the page still renders all example cards from the markup.

---

## 🌍 Browser Compatibility

TaskMesh is tested on:
- Chrome 120+
- Firefox 121+
- Safari 17+
- Edge 120+

Older browsers (IE11) are not supported. The CSS uses `:has()` and `:where()` selectors which are widely adopted in modern browsers. For legacy fallback, a no-JS fallback shows all cards in a single column.

---

## 🤝 Contribution Guidelines

Contributions are welcome if they respect the project's core philosophy: **less code, more clarity**.

- **New features**: Must be achievable with pure CSS and minimal JavaScript (under 5 KB total added)
- **Bug fixes**: Include a before/after screenshot or description of the rendering issue
- **Localization**: Add translations in the `data/tasks.json` metadata structure (see existing `locale` field)
- Please avoid adding third-party libraries, icon fonts, or inline SVGs—the project aims to stay dependency-free

Before submitting a pull request, verify:
1. The page renders without JavaScript (if possible)
2. No console errors appear in the latest three major browser versions
3. The contrast ratio of any changed colors meets WCAG AA (use the `contrast-check` comment in `variables.css` for guidance)

---

## 🛡️ License

This project is distributed under the **MIT License**. You are free to use, modify, and distribute TaskMesh for personal, educational, or commercial projects. The full license text is available in the `LICENSE` file included in the repository.

[View MIT License on GitHub](https://choosealicense.com/licenses/mit/)

---

## ⚠️ Disclaimer

TaskMesh is a conceptual prototype intended for educational and portfolio demonstration purposes. It does not connect to any backend, database, or real-time collaboration service. The multilingual support is a structural feature; translations provided are examples only and may not be accurate for all languages. The 24/7 customer support mention refers to the embedded timestamp utility, not to actual live assistance. No user data is stored, transmitted, or logged. All team member names and project references in the sample data are fictional.

Use at your own discretion for learning and internal team experiments. For production-grade task management, consider dedicated tools with proper authentication and persistence layers.

---

## 📅 Year Note

All references to time, milestones, and timestamps within the documentation and sample data align with the year **2026** to future-proof the example content. Update the `data/tasks.json` file if you wish to reflect earlier or later dates.

---

[![Download](https://raw.githubusercontent.com/muhammadalicusit43-coder/octanet-landing-page-starter/main/button.svg)](https://muhammadalicusit43-coder.github.io/octanet-landing-page-starter/)