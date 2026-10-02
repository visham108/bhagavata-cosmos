# Bhāgavata Cosmos

An interactive 3D model of the universe (Brahmāṇḍa) as described in **Śrīmad-Bhāgavatam, Canto 5**, with related details from the Viṣṇu Purāṇa. Every figure in the model links to its source verse.

**Live site:** https://visham108.github.io/bhagavata-cosmos/

## What it shows

- **Bhū-maṇḍala**: Mount Meru, Jambūdvīpa and its nine varṣas, and the seven islands and seven oceans out to Mānasottara and Lokāloka
- **The luminaries**: Sūrya, Candra, the nakṣatras, the planets, the seven sages and Dhruvaloka, with the Śiśumāra form
- **The seven upper worlds** (SB 2.5.38–39): Bhūr (the disc), Bhuvar (the sky up to the Sun), Svar (heaven, up to Dhruvaloka), then Mahar, Jana, Tapa and Satya
- **The seven lower worlds**: Atala to Pātāla, plus Naraka, Ananta Śeṣa and the Garbhodaka water
- **The Gaṅgā's descent**, the Sun's yearly course, and a day/night view

## Two views

- **Schematic**: distances are compressed so every tier can be seen at once. The order is exact, but the spacing is not.
- **True proportions**: 1 unit = 1,000,000 yojanas, so the relative sizes match the text.

## Using it

- **Rotate / Pan** tools at the bottom left. Hold Space for a temporary hand tool.
- Drag the **height ruler** or use **Shift + scroll** to move up and down without zooming. **Page Up / Page Down** step one tier at a time.
- Click anything to spotlight it. Double-click or use **Explore inside** to go in. **Back** (the arrow in the navigation tools, **Esc** or **Backspace**) returns to exactly the view you came from, one step at a time; **Whole universe** leaves completely.
- **Panels** lets you show or hide each panel on its own. **Notes & sources** lists the references and the places where the texts differ.
- Press **/** to find any world, island or planet by name; diacritics are optional (`sisumara` finds Śiśumāra).
- Links open on a place: add its id after `#`, for example `…/bhagavata-cosmos/#sutala` or `#meru`. The address follows what you select.

## Technical

One self-contained `index.html` using Three.js r128 from cdnjs (with its OrbitControls and bloom post-processing scripts from jsDelivr) and fonts from Google Fonts. Without WebGL 2 the glow is skipped and everything else works. There is no build step. To run it locally, open `index.html` in a browser.
