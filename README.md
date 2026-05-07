[README.md](https://github.com/user-attachments/files/27473494/README.md)
# Mon Arc

A single-page, fully customizable goal tracker. No backend, no signup, no tracking — everything lives in your browser.

You define a period of time (your "arc"), break it down into floating bubbles representing the areas of your life or project, and watch your progress unfold day by day.

---

## Live demo

[View it live on GitHub Pages](#) *(replace with your URL)*

---

## What it does

**Mon Arc** is a deliberate, focused space for tracking a personal arc — a 30, 60, 90 day period (or any duration) during which you commit to specific areas of growth, work, or attention.

Two complementary views work together:

- **Bubbles view** — a constellation of draggable, throwable bubbles representing the domains you care about. Click any bubble to write notes, set its importance, or rename it.
- **Calendar view** — a visual grid of your time, day by day, week by week, or month by month. Past time is filled, the present pulses, the future waits.

Everything is customizable. Everything is saved locally. Nothing leaves your machine.

---

## Features

### Customization
- **Editable title** — the middle word is automatically highlighted in italic accent color (e.g. *Spring **fucking** ARC*)
- **Editable subtitles** — text above and below the main title
- **Editable dates** — start and end of your arc, with French month markers auto-generated for the progress bar
- **7 color themes** — mauve, blue, pink, green, red, orange, gold. Every UI element re-tints to match.

### Bubbles
- Up to **8 bubbles**, arranged in a circle that auto-scales with the count
- **Click** any bubble to open its notes panel — write your notes, give it a title, choose its importance
- **Drag** a bubble to throw it around — it has physics and bounces softly back
- **Three importance levels** — small (low), medium, large (high) — each bubble's size reflects its priority
- **Hover** to see which bubble is active

### Calendar
- **Day / Week / Month** granularity toggle
- **Past** bubbles are filled with theme color
- **Today** glows softly with a pulsing animated halo
- **Future** bubbles are dotted outlines, waiting their turn
- **Hover any bubble** to see the exact date, week range, or month
- Auto-refreshes every minute (so the "today" bubble advances at midnight)

### Persistence
- Everything is saved to your browser's `localStorage`
- Your data is **only on your machine** — no server, no account
- Use **Export** to download a JSON backup of your full configuration and notes
- Use **Import** to restore from a backup or transfer to another browser

### Design
- Custom cursor (circle + dot, blends with the background)
- Twinkling starfield in the background
- All animations are tuned to feel calm rather than busy
- Fully responsive (down to mobile, with adapted controls)
- Brussels timezone for date math (you can change this in the source if needed)

---

## How to use it

### First time
1. Open the page in your browser
2. Click the **gear icon** in the bottom-right corner
3. Set your title, dates, and pick a color theme
4. Click each bubble to give it a name and a brief intent

### Day to day
- Click a bubble whenever you want to add notes, reflect, or change importance
- Switch to the **Calendar view** in the top bar to zoom out and see your progress over time
- The day counter and progress bar update live

### Backup / transfer
- Open the gear menu → click **Export** to download a JSON file
- To restore: click **Import** and pick that JSON file
- The page reloads with your imported state

### Reset
- Open the gear menu → click **Reset** twice (the second click confirms)
- All settings and notes wipe back to defaults

---

## Setup (for hosting on GitHub Pages)

```bash
# Clone or download this repo
git clone https://github.com/yourusername/mon-arc.git
cd mon-arc

# That's it. There's no build step — it's a single HTML file.
```

To host it on GitHub Pages:

1. Push to a public repo
2. Go to **Settings → Pages**
3. Set the source to **main branch / root**
4. Wait a minute, then visit `https://yourusername.github.io/mon-arc/`

The file is `spring-fucking-arc.html` (or rename it to `index.html` for a cleaner URL).

---

## Tech

- Pure **HTML / CSS / JavaScript** in a single file
- No frameworks, no build tools, no dependencies
- ~2700 lines, all self-contained
- Canvas API for the bubbles and starfield
- CSS custom properties for theming
- `localStorage` for persistence
- ~50KB total

The whole thing is one file you can open with a double-click — no server needed.

---

## Privacy

Nothing is sent anywhere. Ever.

- No analytics
- No tracking
- No cookies (other than `localStorage`, which never leaves your browser)
- No external API calls
- No fonts loaded from the internet *(if Google Fonts are used in the file, they can be replaced with system fonts)*

If you clear your browser data, your arc data goes with it. Use **Export** regularly if your arc matters to you.

---

## Browser support

Tested on recent versions of:
- Chrome / Edge
- Firefox
- Safari (desktop + iOS)

Requires a browser with `localStorage`, `Canvas`, and CSS custom properties — anything from the last 5 years should work.

---

## Inspiration

This grew out of a personal need to track a 90-day period with intention rather than checkbox-style productivity tools. The bubbles aren't tasks — they're domains of attention. The calendar isn't a deadline tracker — it's a way to feel time passing.

Use it however you like.

---

## Contributing

It's a personal project, but if you fork it and build something cool, I'd love to see it. Open an issue or send a link.

Ideas welcome:
- More themes
- Different layouts (timeline, radial calendar, etc.)
- Optional encryption for the localStorage data
- A mobile-first version with vertical bubbles

---

## License

To be decided.
