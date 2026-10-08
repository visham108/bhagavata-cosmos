# Bhāgavata Cosmos

An interactive 3D model of the universe (Brahmāṇḍa) as described in **Śrīmad-Bhāgavatam, Canto 5**, with related details from the Viṣṇu Purāṇa. Beyond the shell it follows SB 10.89 and the Brahma-saṁhitā and Caitanya-caritāmṛta. Every figure in the model links to its source verse.

**Live site:** https://visham108.github.io/bhagavata-cosmos/

## What it shows

- **Bhū-maṇḍala**: Mount Meru, Jambūdvīpa and its nine varṣas, and the seven islands and seven oceans out to Mānasottara and Lokāloka
- **The luminaries**: Sūrya, Candra, the nakṣatras, the planets, the seven sages and Dhruvaloka, with the Śiśumāra form
- **The seven upper worlds** (SB 2.5.38–39): Bhūr (the disc), Bhuvar (the sky up to the Sun), Svar (heaven, up to Dhruvaloka), then Mahar, Jana, Tapa and Satya
- **The seven lower worlds**: Atala to Pātāla, plus Naraka, Ananta Śeṣa and the Garbhodaka water
- **The Gaṅgā's descent**, the Sun's yearly course, and a day/night view
- **Garbhodakaśāyī Viṣṇu**: below the lower worlds, the second puruṣa lies on Śeṣa in the water He filled half the universe with, the lotus stem rising from His navel (SB 3.8.23–31, 3.20.15–16; CC Ādi 5.95–103). He is drawn as a form of light until a painting is added.
- **Beyond the universe**: zoom out past the shell, or press **Beyond** for Arjuna's journey (SB 10.89). It passes the seven coverings, each ten times thicker than the last and drawn on a log scale (SB 2.2.28–30, 3.11.41). Just outside them is the Causal Ocean, the Virajā (CC Madhya 20.269), where Mahā-Viṣṇu lies on Ananta Śeṣa breathing universes out and in (SB 10.89.52–56; BS 5.47–48; CC Ādi 5.65–70); our universe and countless others, ours the smallest, lie on its waters around Him (SB 3.20.15; CC Madhya 21.84–86). Last are the brahmajyoti, the Vaikuṇṭha planets and Goloka, arranged as the Brahma-saṁhitā ranks the realms (BS 5.2–5, 5.43). None of this is to scale; each step outward is drawn about ten times larger than the last. A first visit opens with a short descent from the whole creation into our universe (any touch, scroll or key skips it).

## Two views

- **Schematic**: distances are compressed so every tier can be seen at once. The order is exact, but the spacing is not.
- **True proportions**: 1 unit = 1,000,000 yojanas, so the relative sizes match the text.

## Using it

- **Rotate / Pan** tools at the bottom left. Hold Space for a temporary hand tool.
- Drag the **height ruler** or use **Shift + scroll** to move up and down without zooming. **Page Up / Page Down** step one tier at a time.
- Click anything to spotlight it. Double-click or use **Explore inside** to go in. **Back** (the arrow in the navigation tools, **Esc** or **Backspace**) returns to exactly the view you came from, one step at a time; **Whole universe** leaves completely.
- **Panels** lets you show or hide each panel on its own. **Notes & sources** lists the references and the places where the texts differ.
- Press **/** to find any world, island or planet by name; diacritics are optional (`sisumara` finds Śiśumāra).
- Links open on a place: add its id after `#`, for example `…/bhagavata-cosmos/#sutala`, `#meru`, `#mahavisnu` or `#goloka`. The address follows what you select.

## Technical

One `index.html`, with two paintings in `img/` (Mahā-Viṣṇu on Ananta Śeṣa, and Ananta Śeṣa bearing the universe), loaded as textures; if they fail to load, drawn figures stand in. It uses Three.js r128 from cdnjs (with its OrbitControls and bloom post-processing scripts from jsDelivr) and fonts from Google Fonts. Without WebGL 2 the glow is skipped and everything else works. There is no build step. To run it locally, serve the folder (for example `python3 -m http.server`) and open it in a browser; opened straight from disk, browsers block the paintings and the drawn figures appear instead.
