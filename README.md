# Dutch Verb Trainer

**[▶ Open live](https://kopalych1.github.io/dutch-verb-trainer/)**

A single-page app for practising Dutch verb conjugations. No frameworks, no dependencies — just one HTML file you can open in a browser or host anywhere.

## Features

- **All major tenses** — present simple, past simple, present perfect
- **Irregular and regular verbs** — 55+ verbs from the standard Dutch curriculum
- **hij/zij disambiguation** — singular (he/she) and plural (they) are shown separately
- **Inline pronoun display** — pronoun sits left of the input field so you always know what you're conjugating
- **Instant feedback** — correct answer shown on mistakes, mistake list at the end
- **Best score** saved in localStorage
- **EN / NL interface** — toggle between English and Dutch UI, Dutch is the default
- **Mobile-friendly** — responsive layout, works on phone and desktop
- **Keyboard-first** — Enter to check, Enter again to move to next question

## Usage

Just open `index.html` in a browser. No build step, no server needed.

To host it:
- **GitHub Pages** — push the file and enable Pages in repo settings
- **Netlify** — drag and drop the file
- **Any static host** — upload the single file

## Structure

Everything lives in `index.html`:

```
index.html
├── CSS variables + styles
├── Setup screen   (verb selection, tense, order)
├── Quiz screen    (pronoun tag + input row)
├── Results screen (score, mistakes review)
└── JS             (verb data, i18n, quiz logic)
```

## Verb data

Verbs are split into two sets:

- `IRREGULAR` — ~55 verbs (beginnen, zijn, hebben, gaan, …)
- `REGULAR` — ~15 verbs (werken, leren, praten, …)

Each verb has full conjugation tables for present, past, and past participle.

## License

MIT
