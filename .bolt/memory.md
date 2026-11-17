# Project memory

## Product intent & audience

- Single-file portfolio website for a marketer actively seeking employment and applying for marketing positions.
- Audience: hiring managers, recruiters, and marketing team leads at companies reviewing candidates.
- Goal: present skills, case studies, and certifications as a job-seeking showcase.

## Brand personality & voice

- Energetic, creative, modern, and professional marketing tone.
- Bilingual leaning: English with Vietnamese section labels (e.g., About / Giới thiệu, Skills / Kỹ năng, Case Studies / Dự án, Certifications / Chứng chỉ, Contact / Liên hệ).
- Placeholder persona used: "Minh Anh Trần" — real name, bio, and project details to be swapped in later.

## Visual design & UX direction

- Bold, vibrant palette: electric blue, coral, neon accents, gradient combinations.
- Asymmetric grid layouts to convey creativity; glassmorphism (frosted dark cards) for skills and navbar.
- Google Fonts via CDN; strong typographic hierarchy.
- Animations: drifting gradient blobs, floating particles, typewriter effect for job titles, scroll-triggered fade/slide reveals via Intersection Observer, animated number counters for stats.
- Micro-interactions: hover lift on cards, hoverable skill tags, progress bars animating on scroll, form validation with green/red borders and shake animations on errors.
- Sticky navbar becomes frosted-glass on scroll; active link highlighting via scroll position; mobile hamburger menu.
- Honors `prefers-reduced-motion` for all animations.
- Fully responsive via Flexbox/Grid and media queries across mobile, tablet, desktop.

## Decisions, constraints & rationale

- Strict single `.html` file: all CSS in `<style>`, all JS in `<script>`; no frameworks or libraries (Google Fonts CDN only).
- No external animation/scroll libraries; Intersection Observer API used instead.
- Section order fixed: Hero → About → Skills → Case Studies → Certifications → Contact.
- Placeholder content written in realistic professional marketing context (metrics like "+150% traffic", "4.2x ROAS"; certs: Google Ads, Meta Blueprint, HubSpot, GA4).
- Removed default scaffold files after building the single-file portfolio; build passes.

## Open questions & assumptions

- Real marketer identity, bio, and project details are pending; current content is a realistic placeholder.
- Language mix assumption: bilingual English/Vietnamese headers acceptable unless user requests a single language.
- Contact form is non-functional by default ("functional-looking"); no backend specified yet.
- Profile photo is a styled avatar/initials placeholder; real photo not provided.