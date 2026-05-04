# 03 — Step-by-Step Execution

## Workflow: Plan-First + RTCC-O

---

## Step 1: Define Requirements (RTCC-O)
- ✅ Baca CV Fahmi secara lengkap
- ✅ Identifikasi semua experience, skill, sertifikasi
- ✅ Tentukan target audience (recruiter tech/digital)
- ✅ Buat RTCC-O prompt yang spesifik

## Step 2: Design Decisions
- ✅ Pilih aesthetic: Dark editorial + tech terminal
- ✅ Pilih font pairing: Syne + DM Mono + Fraunces
- ✅ Define color palette dengan CSS variables
- ✅ Sketch mental wireframe per section

## Step 3: HTML Structure (Semantic)
```
Dibuat section by section:
[x] nav — fixed navbar dengan logo + links + hamburger
[x] section#hero — nama, tagline, CTA buttons, badge, meta info
[x] section#about — grid layout, about text, 4 stats cards
[x] section#experience — timeline cards, edu card
[x] section#skills — 3 skill cards + proficiency bar section
[x] section#projects — certifications grid (12 cards)
[x] section#contact — CTA section dengan email + LinkedIn
[x] footer — copyright + back to top
```

## Step 4: CSS (Mobile-First)
```
[x] CSS Variables setup
[x] Reset & base styles
[x] Custom cursor styles
[x] Scroll reveal animations
[x] Layout container
[x] Section shared styles (tag, title, em)
[x] Navbar — default transparent → scrolled state
[x] Mobile menu
[x] Hero section — blob, grid bg, animations
[x] About section — responsive grid, stats
[x] Experience — timeline, edu card
[x] Skills — card grid, progress bars
[x] Certifications — responsive grid, provider badges
[x] Contact — radial gradient bg
[x] Footer
[x] Responsive breakpoints (480px, 600px, 768px, 900px)
```

## Step 5: JavaScript (Vanilla)
```
[x] Custom cursor — mousemove tracking + RAF trail
[x] Cursor hover effect on interactive elements
[x] Navbar scroll state
[x] Hamburger toggle
[x] IntersectionObserver untuk scroll reveal
[x] IntersectionObserver untuk skill bar animation
[x] Active nav link highlighting
```

## Step 6: Content Entry
```
[x] Hero: nama lengkap, tagline 3 roles, sub description
[x] About: 2 paragraf summary, 4 stats (26 APIs, 40%, 200+ users, 3.64 GPA)
[x] Experience: PT PAL (3 bullets), Metrodata (4 bullets) + tags
[x] Education: Brawijaya + GPA + courses
[x] Skills: Technical (7), Tools (6 categories), Soft Skills (7)
[x] Proficiency bars: 6 skills
[x] Certifications: 12 cards dengan provider color coding
[x] Contact: email + LinkedIn
```

## Step 7: QA Checklist
- ✅ Semantic tags: nav, main, section, footer, article, h1-h4
- ✅ Mobile responsive (test di 375px, 768px, 1200px)
- ✅ All links have href
- ✅ Images have alt text (no images used — all CSS)
- ✅ Color contrast accessible
- ✅ Smooth scroll behavior
- ✅ Animations don't block interaction
- ✅ Code readable dan bisa dijelaskan

---

## Semantic HTML Tags yang Digunakan

| Tag | Lokasi | Fungsi |
|-----|--------|--------|
| `<nav>` | Fixed navbar | Navigasi utama |
| `<main>` | Wrap all sections | Konten utama halaman |
| `<section>` | hero, about, experience, skills, projects, contact | Setiap segment konten |
| `<article>` | Timeline items | Setiap entry experience |
| `<footer>` | Bottom | Copyright & links |
| `<h1>` | Hero name | Nama utama (1 per page) |
| `<h2>` | Section titles | Judul tiap section |
| `<h3>` | Role titles, card titles | Sub-headings |
| `<h4>` | Cert card titles | Tertiary headings |
| `<ul>/<li>` | Nav, bullets, skill lists | List content |

---

## Responsive Breakpoints

| Breakpoint | Changes |
|------------|---------|
| `< 480px` | Single column everything, smaller hero text |
| `≥ 600px` | 2-col certs grid, 3-col skills grid |
| `≥ 768px` | Nav links visible, about 2-col grid, hamburger hidden |
| `≥ 900px` | 3-col certs grid |
