# 02 — Project Details (RTCC-O)

## Identitas Proyek
| Field | Detail |
|-------|--------|
| Nama Proyek | Portfolio Website — Muhammad Fahmi G.G. |
| Tipe | Static Website (HTML/CSS/JS) |
| Hosting Target | GitHub Pages |
| Deadline | KAreerr Elevation Vol. 2 submission |

---

## RTCC-O Framework Applied

### R — Role
> "mid-level system analyst, frontend developer, dan UI/UX designer yang membangun portfolio untuk fresh graduate tech yang ingin menonjol di mata recruiter."

### T — Task
> "Buat portfolio website lengkap dengan: hero section, about, experience timeline, skills dengan visual bars, certifications grid, dan contact section. Deploy-ready di GitHub Pages."

### C — Context
**Tentang Fahmi:**
- Fresh graduate Computer Engineering Brawijaya University (GPA 3.64/4.00)
- 2 pengalaman internship: PT PAL Indonesia (System Analyst) & Metrodata Academy (App Developer)
- Skill mix: BA/SA + API development + UI/UX design
- 13+ sertifikasi aktif (IBM, Dicoding, RevoU, dll)
- Target role: System Analyst, Business Analyst, Junior Developer

**Tech Context:**
- Pure HTML5 + CSS3 + Vanilla JS
- Google Fonts (Syne, DM Mono, Fraunces)
- Intersection Observer API untuk animations
- CSS Custom Properties untuk theming

### C — Constraints
**WAJIB ada:**
- Semantic HTML5: `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`
- Responsive CSS dengan mobile-first approach
- Semua code harus bisa dijelaskan ke recruiter (no magic/obfuscation)
- Performance: no heavy libraries

**TIDAK boleh:**
- Framework berat (React, Vue, Angular)
- jQuery atau library besar lain
- CSS framework seperti Bootstrap (bisa pakai custom Tailwind-style)
- Gambar dari external CDN yang bisa broken

### O — Output
```
portfolio/
├── index.html       # Main portfolio page (semantic HTML5)
├── style.css        # Mobile-first responsive stylesheet
├── assets/          # Screenshots + images
│   ├── desktop-view.png
│   └── mobile-view.png
└── plan/
    ├── 01-brainstorm.md
    ├── 02-details.md
    ├── 03-execution.md
    └── 04-results.md
```

---

## Technical Specifications

### HTML Structure
```html
<body>
  <nav>           <!-- Fixed navigation bar -->
  <main>
    <section id="hero">        <!-- Landing / hero -->
    <section id="about">       <!-- Summary + stats -->
    <section id="experience">  <!-- Timeline + education -->
    <section id="skills">      <!-- Skill cards + bars -->
    <section id="projects">    <!-- Certifications grid -->
    <section id="contact">     <!-- Contact CTA -->
  </main>
  <footer>        <!-- Copyright + back to top -->
</body>
```

### CSS Architecture
- CSS Custom Properties (variables) untuk semua colors, spacing
- Mobile-first: base styles untuk mobile, `@media (min-width: ...)` untuk desktop
- BEM-inspired naming: `.section-title`, `.tl-header`, `.cert-card`
- No `!important` abuse — specificity dikelola dengan struktur

### JS Features (Vanilla)
1. **Custom cursor** — mouse tracking + trail animation
2. **Navbar scroll** — add `.scrolled` class after 60px scroll
3. **Hamburger menu** — toggle mobile nav
4. **Scroll reveal** — IntersectionObserver untuk fade-in elements
5. **Animated skill bars** — width transition triggered on scroll
6. **Active nav link** — highlight berdasarkan current section

---

## Color Palette
| Variable | Value | Usage |
|----------|-------|-------|
| `--bg` | `#090b10` | Main background |
| `--accent` | `#5af0a4` | Electric green — CTAs, highlights |
| `--accent2` | `#7b8aff` | Periwinkle — secondary accents |
| `--text-primary` | `#eef0f6` | Main text |
| `--text-secondary` | `#8a93a8` | Body text |

## Typography
| Font | Usage | Personality |
|------|-------|-------------|
| Syne | Headers, nav, buttons | Bold, geometric, modern |
| DM Mono | Body text, tags | Technical, clean, readable |
| Fraunces | Italic accents in titles | Elegant contrast |
