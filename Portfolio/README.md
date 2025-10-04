# Retro Portfolio — Setup & Notes

This folder contains a handcrafted personal portfolio built with **HTML, CSS, and vanilla JavaScript**. The visual language mixes old-book textures, typewriter headings, and playful pixel labels to match the desired retro aesthetic.

## Structure

| File         | Purpose                                                                                                |
| ------------ | ------------------------------------------------------------------------------------------------------ |
| `index.html` | Semantic layout for the homepage (hero, about, skills, projects, labs, testimonials, contact, footer). |
| `styles.css` | Global styling, typography, layout, responsive tweaks, animations.                                     |
| `script.js`  | Navigation toggle, scroll-reveal observer, micro-interactions, automatic year stamp.                   |

## How to Preview

Open `index.html` in any modern browser. For the best experience, serve the folder through a lightweight web server so that relative links resolve cleanly:

```bash
# using Python 3
python -m http.server 8080
```

Navigate to `http://localhost:8080/Portfolio/`.

> ℹ️ Command shown for reference; run it from the project root in a shell that supports Python.

## Customization Checklist

- **Hero & About copy**: Update bio text, stats, and CTA destinations inside `index.html`.
- **Project cards**: Swap placeholder entries with real project details, screenshot links, or GitHub/live URLs.
- **Contact details**: Replace social handles and email with personal links.
- **Color palette & fonts**: Adjust CSS variables at the top of `styles.css` or change Google Fonts in the `<head>`.
- **Animations**: Tune transition speeds or remove scroll reveals in `script.js` if needed.

## Assets & Credits

- Background textures use free patterns hosted by [Transparent Textures](https://www.transparenttextures.com/) (public domain). Replace with local files if you need full offline support.
- Portrait photo is a temporary Unsplash placeholder. Swap it with a personal image for final submission.

## Accessibility & Responsiveness

- Semantic landmarks (`<header>`, `<main>`, `<section>`, `<footer>`) structure the page.
- Keyboard and screen-reader friendly mobile navigation (aria attributes + focus states).
- Works on desktop, tablet, and mobile via flex/grid layouts and media queries.
- `prefers-reduced-motion` is respected: the site disables flip animations for motion-sensitive users.

## Next Ideas

- Add a blog page with markdown-to-HTML build step.
- Wire the contact form to a service like Formspree or a custom backend.
- Create a `now` page or roadmap timeline to spotlight current learning goals.
