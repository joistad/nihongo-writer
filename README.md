# Nihongo Writer

Turn any Japanese words into Anki flashcards that teach you how to write them.

**Live app:** https://www.perplexity.ai/computer/a/nihongo-writer-oyuZw3UiQb2FanK.AIKigg

## Features

- Generates `.apkg` Anki decks with animated stroke-order cards (powered by HanziWriter)
- Supports all three Japanese writing systems: kanji, hiragana, katakana
- Automatic readings & meanings via the Jotoba API
- Pitch accent coloring (heiban / atamadaka / nakadaka / odaka / kifuku) — strokes are also colored to match
- Optional word audio via Google Cloud Text-to-Speech
- Suggested word lists: JLPT N5–N1, Joyo grades, frequency lists (Kaishi 1.5k, Core 2k/6k/10k), Kanken levels 10–2
- Dark mode

## Usage

1. Open the live app
2. Type or paste Japanese words (separated by spaces or new lines), or pick from a suggested word list
3. Optionally expand "Want to add word audio?" and paste a Google Cloud TTS API key
4. Click **Download Anki Deck** — import the `.apkg` file into Anki

## Stack

Single-file static web app (`index.html`):
- [HanziWriter](https://hanziwriter.org/) — stroke animation
- [sql.js](https://sql.js.org/) — SQLite in the browser (for `.apkg` generation)
- [JSZip](https://stuk.github.io/jszip/) — zip packaging
- [Jotoba API](https://jotoba.de/) — Japanese dictionary
- Google Cloud Text-to-Speech API (optional, user-supplied key)

## Credits

Card template based on [Write-Kanji by krmanik](https://github.com/krmanik/Write-Kanji).
