# Groove CSS experiments

Small collection of custom CSS experiments for changing the appearance of Groove-style app tiles and icons.

## Files

- `groove-style.css` removes the default tile background to create a more transparent, Windows 10 Mobile-inspired look.
- `groove-style-icons.css` replaces app tile artwork with a set of nostalgic/custom icons for supported apps.
- `groove-icons-testes.css` is explicitly marked as a testing-only variant for icon experiments.

## Quick reference

| File | Purpose | Stability |
| --- | --- | --- |
| `groove-style.css` | Transparent tile styling | Stable experiment |
| `groove-style-icons.css` | Custom icon replacements | Stable experiment |
| `groove-icons-testes.css` | Trying icon changes before promoting them | Testing only |

## Current icon targets

The icon stylesheet includes selectors for apps such as Instagram, Reddit, Discord, YouTube, Play Store, Spotify, X, Pinterest, WhatsApp, TikTok, SpaceHey Mobile and GitHub.

## Usage

These files are standalone CSS customizations. Use the stylesheet that matches the visual change you want, and keep the `*-testes.css` file for experimentation rather than treating it as the stable variant.

For safer experimentation, test changes in `groove-icons-testes.css` first and only copy a selector into `groove-style-icons.css` once the icon renders as expected.

## Maintenance notes

- Keep selectors for different apps separate so one broken rule does not make unrelated icon changes harder to debug.
- When replacing an external icon URL, prefer a direct HTTPS asset URL and verify that it still returns an image before committing the change.
- Some icon assets are loaded from external URLs, so their availability depends on the third-party hosts remaining online.
- The CSS files are kept separate so transparent-tile styling and icon experiments can be used independently.
