# Groove CSS experiments

Small collection of custom CSS experiments for changing the appearance of Groove-style app tiles and icons.

## Files

- `groove-style.css` removes the default tile background to create a more transparent, Windows 10 Mobile-inspired look.
- `groove-style-icons.css` replaces app tile artwork with a set of nostalgic/custom icons for supported apps.
- `groove-icons-testes.css` is explicitly marked as a testing-only variant for icon experiments.

## Current icon targets

The icon stylesheet includes selectors for apps such as Instagram, Reddit, Discord, YouTube, Play Store, Spotify, X, Pinterest, WhatsApp, TikTok, SpaceHey Mobile and GitHub.

## Usage

These files are standalone CSS customizations. Use the stylesheet that matches the visual change you want, and keep the `*-testes.css` file for experimentation rather than treating it as the stable variant.

## Notes

Some icon assets are loaded from external URLs, so their availability depends on the third-party hosts remaining online. The CSS files themselves are kept separate so the transparent-tile styling and icon experiments can be used independently.
