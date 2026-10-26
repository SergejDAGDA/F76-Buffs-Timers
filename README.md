# Fallout 76 Buff Timers

A browser-based utility for tracking XP and Intelligence buffs in Fallout 76, with live timers and an XP calculator.

## Project status

**Legacy prototype.** The current implementation is a single `index.html` file supported by resources in `Assets/`. It needs a broader review before further development. Buff values, durations, and gameplay assumptions have **not** been revalidated against current Fallout 76 updates, so do not treat them as authoritative.

This README documents the current baseline. It does not change the application or claim that its calculations have been recently tested.

## Preview locally

No build configuration is included. To preview the existing static page, download or clone this repository, then run a simple static server from its root:

```sh
python -m http.server 8000
```

Open `http://localhost:8000` in your browser. You can also try opening `index.html` directly, although a local server is a more representative way to preview a web page.

## Modernization checklist

Before changing the implementation:

- Verify the currently available buffs, their effects, and their durations against the game.
- Review how timers behave after a refresh and across multiple open tabs.
- Review the XP calculator's inputs, assumptions, and edge cases.
- Check mobile usability, accessibility, and keyboard interaction.
- Decide on a small, testable next version before a larger rewrite.

The items above are proposed checks, not a claim that these features are broken.
