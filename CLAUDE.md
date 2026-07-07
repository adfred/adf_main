# anthonydfrederick.com — Project Notes

## What this project is

A rebuild of my personal site, currently live at **anthonydfrederick.com**, hosted on
GoHighLevel (an all-in-one coaching platform I'm cancelling). The goal is a plain
HTML/CSS/JS static site, no framework, no build step, deployable directly on
GitHub Pages.

This is a **brand-new repo** — nothing exists yet. Part of this project is setting
up the repo itself (see "Repo setup" below) before any site code gets written.

**Priority: match the existing live site's text content, structure, and layout.**
Before writing any page, look at the real thing first — don't work from memory or
assumption.

## Scope — read this before doing anything else

**Only these four pages get rebuilt:**
- Home (`index.html`)
- About (`about.html`)
- Coaching (`coaching.html`)
- Work (`work.html`)

Do not build Resources or Cart pages or any related structure (no cart logic,
no product listings) — they're out of scope for now. Don't build Privacy or
Terms pages either unless I ask.

**Do not try to recreate any graphical elements** — logos, icons, sprite/line-art
marks, photos, or any other imagery. I have the real media files for this
project in a folder on my desktop and will hand them over separately.

Instead:
- Leave a clearly-labeled placeholder wherever an image belongs (a simple gray
  box or `<!-- IMAGE: description of what goes here -->` is fine), sized and
  positioned correctly for the layout.
- Don't hand-draw or approximate logos/icons in SVG or CSS. If the original
  uses an icon or animated mark, just note "icon goes here" as a placeholder
  and move on — I'll drop in the real graphic later.
- Focus your effort on getting the **text content, typography, spacing, color,
  and layout structure** right — that's the part actually worth rebuilding by
  hand.

## Workflow — please follow this loop

1. Visit the live page on **anthonydfrederick.com** (or the specific sub-page).
2. Screenshot it — desktop width and mobile width.
3. Build/update the matching local page — text, layout, and structure only,
   with placeholders standing in for any graphics per the Scope section above.
4. Screenshot your local result at the same widths.
5. Compare the two screenshots side by side for layout, spacing, type, and
   color match (ignore the fact that placeholders aren't real images). Keep
   iterating before moving on if something's off.
6. Only move to the next page once the current one is a close match.

Don't tell me a page is done until you've actually done this comparison yourself.

## Known design system (confirmed from the live site)

- **Two background modes:**
  - Dark forest-green (`~#142118`) with warm cream text (`~#fef1e2`) — used on
    Home, Coaching, About (top), Work (project-listing section)
  - Warm cream (`~#fef1e2`) with dark forest-green text (`~#142118`) — used on
    the About page
  - Gold/yellow accent (`~#fcd762`) for solid buttons on paper sections
- **Type:** "Rubik" fontface

Verify all of this against the live site rather than trusting this list
blindly — it was reconstructed from screenshots, not the original source, so
treat it as a starting point, not ground truth.

## Site structure

- `index.html` — Home: hero text + links to each section (image/icon
  placeholders where the animated marks belong)
- `about.html` — hero image, "Hi friend" personal letter, coaching CTA,
  newsletter/booking/contact CTAs
- `coaching.html` — Inner Life Coaching, testimonials, 45-minute session
  offer
- `work.html` — Film Work: Scripted/Unscripted project
  lists

## Content notes / things to get right

- **Newsletter** links to Substack (`https://anthonydfrederick.substack.com/`)
  — no Super.site or Cutting Instincts references anywhere.
- **Booking link:** replace every placeholder booking URL with my real
  scheduler link — https://scheduler.zoom.us/anthony-frederick/1-to-1
- **Contact email:** contact@anthonydfrederick.com (Film Work inquiries)

## Repo setup

There is no existing repository — please help me:
1. Initialize a new git repo in this project folder
2. Create a new GitHub repository (I have GitHub connected already)
3. Make an initial commit and push, then continue building on top of it with
   incremental, clearly-messaged commits as pages get built

## Constraints

- No frameworks (no React/Vue/etc.) — plain HTML/CSS/JS only.
- No build step — this should run by just opening the files or serving the
  folder directly, and deploy as-is to GitHub Pages.
- Keep it accessible: visible focus states, alt text placeholders on images,
  respects `prefers-reduced-motion`.
- Commit incrementally with clear messages as you go, rather than one giant
  commit at the end — I want to be able to see progress in the repo history.
