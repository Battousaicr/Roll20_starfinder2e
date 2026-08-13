# Starfinder Second Edition Roll20 — PF2e Presentation Fork v0.1

## What this version is

This is not a reduced or rewritten sheet.

`starfinder2.html` begins with the current public **Pathfinder Second Edition by Roll20**
HTML source and preserves its existing sheet structure, attributes, repeating sections,
roll buttons, NPC sheet, roll templates, and Sheet Worker code.

`starfinder2.css` begins with the current public PF2e CSS source. A Starfinder Second
Edition theme override is appended to the end. This lets us change the presentation
without rewriting the shared PF2e/SF2e engine.

## Deliberate changes in v0.1

1. Replaced the visible Pathfinder logo image in the top-left with a text-only
   `STARFINDER / SECOND EDITION` test mark.
2. Added `attr_sf2e_theme_version=0.1`.
3. Added a Starfinder-themed visual override layer using void blue, tech blue, cyan,
   violet, and magenta accents.
4. No intentional changes to PF2e rules calculations or Sheet Workers.

## Test in Roll20

For a game's **Custom** character sheet:

- Paste `starfinder2.html` into **HTML Layout**.
- Paste `starfinder2.css` into **CSS Styling**.
- Save Changes.
- Open a character.

You should see the same PF2e sheet layout and functionality, but with the Starfinder
test presentation.

`sheet.json` is included for project structure, but the normal Custom Sheet Editor does
not consume it.

## Development rule going forward

When PF2e and SF2e use the same mechanic:
- keep the PF2e attribute
- keep the PF2e roll
- keep the PF2e worker
- change only presentation/visible terminology when necessary

Only genuine SF2e rules differences should cause mechanical code changes.

## Source and license

Base source:
https://github.com/Roll20/roll20-character-sheets/tree/master/Pathfinder%20Second%20Edition%20by%20Roll20

The Roll20 character sheet repository is distributed under the MIT License.
See `LICENSE_ROLL20_SOURCE.txt`.

Official Starfinder branding/art is not bundled in this test package. The temporary
header is text/CSS only.
