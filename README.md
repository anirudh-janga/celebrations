# Celebrations

Interactive festival greetings to send to friends and family. Each festival gets its own folder with a single, self-contained page.

| Festival | Page | Notes |
| --- | --- | --- |
| Diwali 2026 | [`diwali-2026/`](diwali-2026/index.html) | three.js sunset-to-night intro over an Indian city, a Telugu greeting, 12 classic crackers (tarajuvva, chichubuddi, bhoochakram, kakarapuvvottulu…) to burst, a 60-second Roshni round, and a Diwali 2026 almanac with sources. User stories: [`docs/diwali-2026/USER_STORIES.md`](docs/diwali-2026/USER_STORIES.md). |

## Devices

- **iPhone:** plays sound through the silent switch, two-finger lighting, compact landscape layout, no accidental zoom.
- **iPad:** full-quality effects, larger cracker cards, full-screen button.
- **Desktop:** click the street (a ring shows where), keys `1`–`9`, `0`, `-`, `=` pick crackers, `Space` lights at the cursor, `M` mute, `I` almanac, `F` full screen.
- Render resolution and particle density adapt to the measured frame rate.

## Personal greeting

Add `#from-YourName` to a page link and the greeting will say it came from you, for example `.../diwali-2026/#from-Anirudh`. Only letters, numbers and hyphens are read; hyphens become spaces.

## Run locally

No build step. Serve the folder and open it:

```sh
python3 -m http.server 8000
# then open http://localhost:8000/diwali-2026/
```

three.js r128 loads from cdnjs; fonts load from Google Fonts. Sound is synthesized with the Web Audio API, so there are no asset files.

## Publish with GitHub Pages

`.github/workflows/pages.yml` deploys on every push to `main` or the Diwali branch, and can be run by hand from the Actions tab. It publishes `index.html` plus every top-level folder that has an `index.html` (so new festival folders go live automatically), and leaves out `docs/`. In **Settings → Pages**, the source must be set to **GitHub Actions**.

Live at `https://anirudh-janga.github.io/celebrations/`.
