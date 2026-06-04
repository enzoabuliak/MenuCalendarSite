# MenuCalendar — Website

Marketing + privacy + support site for [MenuCalendar](https://github.com/enzoabuliak/MenuCalendar),
a free menu bar calendar app for macOS.

Vanilla static HTML, one shared `assets/site.css`, **no build step.**

## Pages

- `index.html` — landing (hero, popover mock, features, specs, privacy strip, FAQ)
- `privacy.html` — Apple-style plain-language data story
- `support.html` — contact email + bug-report checklist
- `changelog.html` — release notes rendered from `CHANGELOG.md`

## Run locally

```bash
python3 -m http.server 4321
# open http://localhost:4321
```

## Design

Dark-first, Flexoki palette, Space Grotesk + JetBrains Mono. Same family as
[`enzoabuliak/personal-site`](https://github.com/enzoabuliak/personal-site),
pushed toward Apple product-page polish: backdrop-blur sticky header, soft
radial orange glow under the hero, centered hero with one prominent CTA,
SVG mockup of the popover as the screenshot-as-hero placeholder.

The popover mock in the hero is real layout — month nav, 6×7 grid with today
(June 4) highlighted, agenda with three events, a menu-bar sliver above
showing the status item. It'll get swapped for a real recording before v1.

## Deploy

Target: GitHub Pages on the `main` branch.

```
Domain        menucalendar.enzoabuliak.com
Source        github.com/enzoabuliak/MenuCalendarSite
Download zip  github.com/enzoabuliak/MenuCalendar/releases/download/v1.0.0/MenuCalendar-1.0.0.zip
```

DNS setup, the CNAME file, and pushing the app repo are tracked in the
project note (`student-vault/04_Projects/Active/MenuCalendar.md`).
