# Name Picker Party 2

Six more classroom name-picker mini-games, made to be shown on a projector. Same engine and look as [Name Picker Party](https://github.com/pctppsptutor-lab/goi-ten-vui-nhon).

## How to play

Open `index.html` in Chrome or Edge, or use the GitHub Pages link. Add your class with the yellow class button, pick a game at the top, then press **▶ Pick a name!** or Space.

| Game | How it works | Twist |
|---|---|---|
| 07 Sneezing Flower Bee | Ten gardeners stand by their flowers; the bee checks each flower and lands on the chosen one. | The first flower sneezes pollen and blows the bee across the garden onto the real winning flower. |
| 08 Candy Tornado | Candies roll through a chain-reaction machine of rails, jelly springs and chocolate levers into ten cups. | The golden candy hits a fake lollipop and sticks; the candy cat pulls a spare lever and every rail swaps. |
| 09 Hamster Turbo Wheels | Hamsters run in wheels to charge their jars; the first full jar rings the bell. | The fastest wheel spins out and slips backwards; a sunflower seed rolls onto a switch and lights the real winner. |
| 10 The Shape-Shifting Book | Ten pages show their symbols, close and shuffle; the bookmark finds the winning page. | An eraser rubs out the first page's symbol; the glowing bookmark slides to the real page. |
| 11 Capybara Melon Delivery | Capybaras nose watermelons down the canal to the delivery ring. | The first melon splits open with a duckling inside; the current turns and carries another melon in. |
| 12 Popcorn Cinema | Students shake popcorn to the projector's beat; when the music stops the spotlight picks one. | A bucket explodes off the beat; the projector adds a bonus beat and the spotlight moves on. |

About one round in four has no twist. The winner is always chosen the moment you press Pick.

Class lists stay in the browser and are shared with Name Picker Party when both are opened from the same site; use **Export backup** on the class page to keep a copy.

## Folders

- `index.html` – shell (UI, sound, music, camera, class lists).
- `games/` – one file per game, plus `fx.js` (particles, camera), `bases.js` (code-drawn backgrounds) and `scenes.js` (moving scene layers).
- `assets/` – sprites, burst effects and sounds for each game.


## Sound effects

Game-specific MP3 effects load only for the selected game and use the existing Sound toggle and SFX volume. Credits and edit details are in `assets/sfx/credits.html` and `assets/sfx/sources.json`.

Run the dependency-free audio lifecycle checks with `node tests/sfx.test.cjs`.

Music uses original four-phrase pentatonic hooks, recorded VCSL lead instruments and percussion, with synthesized accompaniment as a loading fallback. Foreground effects briefly lower the music and take priority over ambient effects.
