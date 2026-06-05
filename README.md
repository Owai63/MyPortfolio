# MOI.ENG Portfolio v5.0

> Cyberpunk / embedded-systems aesthetic portfolio — Muhammad Owais Iqbal Malik

## File Structure

```
portfolio/
├── index.html        ← main HTML (structure & content only)
├── css/
│   └── style.css     ← all styles, variables, animations, responsive
├── js/
│   └── main.js       ← all interactivity & canvas logic
└── README.md
```

## Sections

| # | Section | Description |
|---|---------|-------------|
| 01 | Experience | 4-entry animated timeline |
| 02 | Skills | Pill grid + radar chart (7 axes) |
| 03 | Projects | Dossier console — filterable index + viewport (11 projects) |
| 04 | GitHub | Live repo grid via GitHub API |
| 05 | Education | Degree + CGPA card |
| 06 | Awards | Gold & Silver medal cards |
| 07 | Certifications | Flip-card carousel (5 certs) |
| 08 | Open To | Role cards — positions open to |
| 09 | Contact | Email, phone, LinkedIn, location |


## Projects

Projects live as data objects in the `DOSSIERS` array in `js/main.js` and render into a filterable dossier console (All / Production / Academic). To add a project, append an object with `id`, `icon`, `cat`, `org`, `title`, `status`, `statusLabel`, `context`, `stack`, `bullets[]`, `tags[]`, and optional `note` / `badge`.

| Project | Category | Org / Context |
|---------|----------|---------------|
| Car Tracker — LTE/BLE/GPS IoT Device | Production | Palmlabs |
| Production Database & Tracker Device Management | Production | Palmlabs |
| Shooting Range Target Control System — XBee & LoRa | Production | Palmlabs |
| Pet Tracker — NB-IoT/LTE-M Asset Tracker | Production | Palmlabs |
| Cedrus Group — Corporate Website | Production | Cedrus Group Internship |
| CareConnect — Hospital Website | Production | Freelance Project |
| Brain-Controlled Wheelchair | Academic | Final Year Project (Gold Medal) |
| Hand Gesture Controlled Car | Academic | Embedded Systems |
| FSM 4-Lane Traffic Light Controller | Academic | Digital Design |
| Bank Management System | Academic | C++ / OOP |
| Online Food Ordering System | Academic | Full-Stack Web |

## Experience Entries

| Company | Role | Period |
|---------|------|--------|
| Palmlabs | Embedded Engineer | Nov 2024 – Present |
| Palmlabs | Systems Administrator | Nov 2024 – Present |
| Northern Mountains Contracting | IT Engineer | Aug 2024 – Nov 2025 |
| Cedrus Group | Web Developer (Intern) | Jun 2023 – Sep 2023 |

## Features

| Feature | File |
|---|---|
| Boot terminal sequence | `js/main.js` |
| Custom crosshair cursor | `css/style.css` + `js/main.js` |
| Mouse trail particles | `js/main.js` |
| Click burst + ripple | `js/main.js` |
| Circuit-board canvas background | `js/main.js` |
| Floating hero particles | `js/main.js` |
| Parallax blobs (mouse-driven) | `js/main.js` |
| 3-D orbital hero visual | `css/style.css` |
| Animated hero stat counters | `js/main.js` |
| Typewriter role subtitle (8 roles) | `js/main.js` |
| Text scramble section headings | `js/main.js` |
| Skill pill stagger entrance | `js/main.js` |
| Skill radar chart — 7 axes (canvas) | `js/main.js` |
| Timeline scan beam | `css/style.css` |
| 4-colour timeline dot progression | `css/style.css` |
| Project dossier console (filterable index + viewport) | `js/main.js` |
| Project category filters (All / Production / Academic) | `js/main.js` |
| Flip certification cards | `css/style.css` |
| Certification carousel with dots | `js/main.js` |
| Mobile tap-to-flip cards | `js/main.js` |
| Live GitHub repository grid | `js/main.js` |
| GitHub repo filter (All / Original / Forks / Starred) | `js/main.js` |
| Active nav highlight on scroll | `js/main.js` |
| Scroll progress bar | `js/main.js` |
| Magnetic CTA buttons | `js/main.js` |
| Audio visualiser bars (awards) | `js/main.js` |
| Open To — role cards section | `css/style.css` |
| Konami code easter egg ↑↑↓↓←→←→BA | `js/main.js` |

## Customisation

All colour variables are at the top of `css/style.css`:

```css
:root {
  --a:   #00ffe0;   /* primary cyan  */
  --a2:  #ff3e6c;   /* accent pink   */
  --gr:  #00ff88;   /* green         */
  --pur: #bd7fff;   /* purple        */
}
```

Timeline dot colours follow the same palette — cyan → pink → green → purple — one per entry. To add a 5th entry, append to `style.css`:

```css
.tli:nth-child(6)::before { background:var(--or); box-shadow:0 0 18px var(--or); }
.tli:nth-child(6) .tli-co { color:var(--or); }
```


## Responsive

- ≥ 1024 px — full two-column layout with orbital visual
- 768 – 1023 px — single column, hamburger menu
- < 768 px — mobile optimised, flip-cards shown flat, tap-to-flip enabled

## Easter Egg

Type the **Konami code** on any page: `↑ ↑ ↓ ↓ ← → ← → B A`
