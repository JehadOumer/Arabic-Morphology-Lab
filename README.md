# Arabic Morphology Lab

Interactive demo of Arabic **root-and-pattern** morphology: how a consonantal root plus a pattern of vowels and affixes yields a family of related words.

This is a **demo release**. It is a static web app and is meant to be used as a guided lesson, not as a complete reference grammar.

**Live demo:** [https://jehadoumer.github.io/Arabic-Morphology-Lab/](https://jehadoumer.github.io/Arabic-Morphology-Lab/)

## What’s in this demo

- **Root × pattern intro** — the idea that ك ت ب (*k–t–b*, writing) can generate many words when vowels and affixes change.
- **Guided k–t–b lesson** — isolated letters fly in, join with Amiri outlines, and receive harakat (short-vowel marks).
- **Pattern set**
  - كَتَبَ *kataba* — he wrote
  - كُتِبَ *kutiba* — it was written
  - كِتَاب *kitāb* — book
  - كَاتِب *kātib* — writer
  - مَكْتُوب *maktūb* — written
  - مَكْتَب *maktab* — office / desk
  - مَكْتَبَة *maktaba* — library / bookshop
  - كُتُب *kutub* — books
  - يَكْتُبُ *yaktubu* — he writes
  - يَكْتُبُونَ *yaktubūna* — they write
- **Learned Patterns bank** — cards accumulate as you move through the lesson; a bottom slider jumps between steps.
- **Skip Animation / Replay** — skip letter-joining on later visits, or replay a word.
- **Transfer root ع م ل** (*ʿ–m–l*, work / action) with two prediction quizzes (عَامِل *ʿāmil* “worker”, مَعْمَل *maʿmal* “factory / laboratory”).
- **Packed-word close** — Qurʾān 15:22 فَأَسْقَيْنَاكُمُوهُ broken into linked pieces (conjunction, verb, subject, objects), with POS/DEP tags and a lexical tooltip.
- **Desktop and phone layouts** — hover on large screens, tap on phones; last-page tooltip as a left card (desktop) or a bottom bar (phone).
- **Dialect map demo** — MADAR CORPUS-25 table view of “This room is too small” across 25 cities ([live](https://jehadoumer.github.io/Arabic-Morphology-Lab/madar-dialect-map.html)).

## Run it locally

This site loads `amiri-forms.json` with `fetch`, so it needs a local server (opening the HTML file directly will miss the outlines).

```bash
python -m http.server 8788
```

Then open [http://127.0.0.1:8788/](http://127.0.0.1:8788/).

## Files

| File | Role |
| --- | --- |
| `index.html` | The morphology lab |
| `madar-dialect-map.html` | MADAR dialect tables demo |
| `amiri-forms.json` | Amiri glyph outlines used to join letters |

Fonts (DM Sans, Amiri, Scheherazade New) are loaded from Google Fonts.
