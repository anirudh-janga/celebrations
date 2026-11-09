# Diwali 2026 page: user stories

The audience is friends and family who open a shared link, usually on a phone, often on a slow connection. They have a minute or two and want to feel the festival. Each story below is small enough to build and test by itself.

Personas used below:

- **Guest**: anyone who opens the link (a cousin in Pune, Nani on her tablet, a friend abroad).
- **Host**: the person who shares the link (the repo owner).
- **Player**: a guest who has started the cracker game.

---

## Epic A: Intro shot, sunset to Diwali night

**A1. Sunset over Seattle**
As a guest, I want the page to open on a wide shot of Seattle at sunset, so that I feel I am on a rooftop on Diwali evening.
- Acceptance: the Space Needle at the end of the street, a downtown tower cluster, the Great Wheel on the waterfront, Elliott Bay, the Olympic Mountains with the sun setting behind them, and Mount Rainier; the camera drifts slowly.

**A2. Sunset fades to night**
As a guest, I want dusk to deepen into night over about 12 seconds, so that the moment the lights come on feels earned.
- Acceptance: the sun sinks below the skyline; the sky passes through pink and violet to deep indigo; stars fade in; the city goes from lit silhouettes to dark shapes.

**A3. The city lights up with diyas**
As a guest, I want thousands of diyas to light up across rooftops, balconies and the street in a ripple, so that the city visibly "wakes up" for Diwali.
- Acceptance: diyas light in a wave from the centre outward; each flame flickers on its own; windows warm up; akash kandils (paper lanterns) and string lights glow on buildings.

**A3b. A different evening every visit**
As a guest who opens the link twice, I want the sky and city to change, so that it feels alive.
- Acceptance: each visit picks one of four sunset palettes (saffron, rose, gold, ember), a sun position, clear or cloudy streaks, and a new layout of buildings and landmarks; a flock of birds crosses the sunset.

**A3d. No flicker**
As a guest, I want the opening shot to be steady, so that it looks polished.
- Acceptance: no shimmering ground or buildings (depth precision, offsets, mipmapped textures, antialiasing on every device); no blurred overlays over the 3D view; no hard-blinking lights.

**A4. The greeting**
As a guest, I want a "Happy Diwali 2026" title with the Telugu greeting "దీపావళి శుభాకాంక్షలు" above it to appear once the city is lit, so that I know what this page is for.
- Acceptance: the title appears after the diyas; the call to action ("Go down to the street") appears below it; the intro can be skipped at any time.

**A5. Personal greeting from the host**
As a host, I want to add my name to the link (for example `#from-Anirudh`), so that guests see "Anirudh wishes you a happy Diwali".
- Acceptance: the name is read from the URL hash, hyphens become spaces, only letters/digits/hyphens are used, nothing is sent anywhere. Without a hash a general greeting shows.

---

## Epic B: The street and the cracker box

**B1. Down to the street (close-up)**
As a guest, I want the camera to swoop from the rooftop view down to a lane lined with houses, rangoli and diyas, so that I am right where the crackers go off.
- Acceptance: a smooth 2–3 second camera move that ends low and close, with a narrower lens, so the lane, rangoli and the fireworks fill the frame; tips sit at the top so the street stays clear; shells burst further down the lane so they stay in view.

**B2. Pick a cracker from the box**
As a player, I want a "cracker box" tray with at least 10 Indian firecrackers, each with a picture and name, so that I can choose what to burst.
- Acceptance: tray scrolls sideways on a phone; each item shows a plain English name, its Telugu name (తారాజువ్వ, చిచ్చుబుడ్డి, భూచక్రం, కాకరపువ్వొత్తులు, పాము బిళ్ళలు…) and a short description in the hint line; the selected item is clearly highlighted.

**B3. Place and light it**
As a player, I want to tap a spot on the street to place the cracker and see its fuse sparkle before it goes off, so that it feels like lighting it with an agarbatti.
- Acceptance: tap places the cracker at that spot; a short fuse sparkle (under 1.5 s) runs before the effect; several crackers can run at once.

**B4. Each cracker behaves like the real thing**
As a player, I want every cracker to have its own effect, so that each one triggers a different memory.
- Rocket: launched from a glass bottle, whistles up, bursts into a peony.
- Flower pot: a tall golden fountain that crackles.
- Ground spinner: spins on the ground throwing a ring of sparks.
- Sparkler: I can drag my finger to write in the air with sparks.
- Bomb: flash, shockwave ring, screen shake and a big boom.
- Cracker chain: a chain of rapid pops crackling down the street.
- Sky shot (12-shot): a series of colourful shells, one after another.
- Bhoochakra/pencil: thin coloured sparks that change colour.
- Snake tablet: a black ash snake that grows and wriggles with smoke.
- Colour matches: little coloured flames.
- Hydrogen bomb / aloo bomb: a heavier bang with smoke.
- Acceptance: each effect is visibly different and lasts 1–6 seconds.

**B5. Nostalgia tidbits**
As a player, I want a short memory or fun fact to pop up when I burst a cracker, so that I smile and remember childhood Diwalis.
- Acceptance: each cracker has 2+ tidbits; one shows in a toast for about 4 seconds; tidbits don't repeat back to back.

**B6. Sound**
As a player, I want whistles, crackles and booms, so that it sounds like Diwali night.
- Acceptance: sound is generated in the browser (no audio files); sound starts only after the first tap; a mute button is always visible.

---

## Epic C: The quick game

**C1. Roshni meter**
As a player, I want a "Roshni" meter that fills as I burst crackers, so that I have a simple goal.
- Acceptance: each cracker adds points; different crackers in a row give a variety bonus; the meter is visible at the top.

**C2. 60-second round**
As a player, I want the round to last about 60 seconds, so that it is quick to play and replay.
- Acceptance: a timer counts down; the round ends when time runs out or the meter is full.

**C3. Grand finale**
As a player, I want a grand finale when I fill the meter, so that I get a big reward.
- Acceptance: the sky fills with a timed multi-shell show; a closing card shows my score, the number of crackers lit, and the greeting with "Play again" and "Copy link" buttons.

**C4. Free play**
As a guest who doesn't want a game, I want to keep bursting crackers without a timer, so that I can just enjoy it.
- Acceptance: a "Free play" option on the start card and after the round.

---

## Epic D: Diwali 2026 in India

**D1. This year's dates**
As a guest, I want to see the five days of Diwali 2026 with dates, so that I know what was celebrated when.
- Acceptance: Dhanteras (Fri 6 Nov), Naraka Chaturdashi/Choti Diwali (Sat 7 Nov), Lakshmi Puja (Sun 8 Nov), Govardhan Puja (Tue 10 Nov), Bhai Dooj (Wed 11 Nov), with a note that some calendars place the last two on 9 and 10 Nov.

**D2. Highlights from this year**
As a guest, I want a short list of what happened in India around Diwali 2026, so that the page feels current.
- Acceptance, each with a source link:
  - First Diwali since Deepavali was inscribed on UNESCO's Intangible Cultural Heritage list (10 Dec 2025, India's 16th element).
  - Ayodhya's 10th Deepotsav on 7 Nov: over 30 lakh diyas reported on the Saryu ghats (reports say up to 36 lakh), beating the 2025 Guinness record of 26,17,215, plus a Ramayana drone show.
  - Supreme Court allowed only certified green crackers in Delhi-NCR on 7–8 Nov (6–7 am and 8–10 pm); ladis and barium crackers stayed banned; the full ban returned 9 Nov.
  - CAIT estimated a record ₹1.25 lakh crore of Dhanteras trade, with gold and silver above ₹66,000 crore and Diwali sales expected to cross ₹7 lakh crore.
  - Kali Puja in Bengal and Bandi Chhor Divas for Sikhs on the same night, 8 Nov.
  - Defence Minister Rajnath Singh spent Diwali with troops in Sikkim.

**D3. Safety note**
As a guest, I want a gentle reminder about safe and green celebrations, so that the page is responsible without being preachy.
- Acceptance: one short card: green crackers, a bucket of water, cotton clothes, keep pets indoors, respect local time limits. Also notes that every cracker on the page is emission-free.

---

## Epic E: Sharing and access

**E1. Works on phones**
As a guest on a phone, I want the whole experience to fit the screen and respond to taps, so that I don't need a computer.
- Acceptance: no horizontal scroll; tray and buttons are thumb-sized; pixel ratio capped at 2; particle counts reduced on small screens.

**E2. Loads fast**
As a guest on mobile data, I want the page to load quickly, so that I don't give up.
- Acceptance: one HTML file plus three.js from a CDN; no images or audio files.

**E3. Copy the link**
As a guest, I want to copy the link with my own name in it, so that I can forward it on.
- Acceptance: a "Share" card with a name field and a copy button that builds `…#from-Name`; falls back to selecting the text if clipboard access is refused.

**E4. Reduced motion**
As a guest who is sensitive to motion, I want camera shake and flashes toned down, so that I can still enjoy it.
- Acceptance: with `prefers-reduced-motion`, no screen shake and softer flashes.

**E5. iPhone**
As a guest on an iPhone, I want sound, taps and layout to just work, so that the experience feels native.
- Acceptance: sound plays through the silent switch (`navigator.audioSession` "playback") and unlocks on the first tap; audio resumes after a call or app switch; pinch and double-tap don't zoom the page; long-press doesn't open a callout; two fingers can light two crackers at once; in landscape a compact tray, HUD and start card fit the short screen; safe-area insets clear the notch and home bar.

**E6. iPad**
As a guest on an iPad, I want full-quality effects and a layout that uses the big screen, so that it looks its best.
- Acceptance: iPads are detected as tablets even though iPadOS reports a Mac; they get the full particle budget and antialiasing; larger tray cards; a full-screen button where the browser allows it.

**E7. Desktop**
As a guest on a computer, I want mouse and keyboard controls, so that I can play without a touchscreen.
- Acceptance: a ring on the street shows where a click will land; keys 1–9, 0, −, = pick crackers (shown as badges on the cards); Space lights at the cursor; M mutes, I opens the almanac, F toggles full screen; the mouse wheel scrolls the tray; a gentle parallax follows the mouse.

**E8. Smooth on every device**
As any guest, I want the animation to stay smooth, so that it never feels laggy.
- Acceptance: the page starts at a quality suited to the device, lowers resolution and then particle density when frames are slow and uneven, and raises them back when things calm down. A steady 30 fps cap (iOS Low Power Mode) is not mistaken for a slow device. Particle buffers aren't re-uploaded while nothing is alive.

**E9. Festival hub**
As a host, I want a home page that lists festival pages, so that future festivals can be added next to Diwali 2026.
- Acceptance: root `index.html` links to `/diwali-2026/`.
