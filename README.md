# Imprecise Precis

A zero-build GitHub Pages manuscript reader prepared to receive a Markdown manuscript.

## Repository state

This repository is intentionally set up with two receptacle files:

- `index.html` — the complete reading/listening application.
- `README.md` — publication and maintenance notes.

The content file is intentionally not present yet.

When the manuscript is ready, add this file at the repository root:

```text
manuscript.md
```

No change to `index.html` is required.

## Manuscript workflow

The reader always loads:

```js
./manuscript.md
```

The first Markdown H1 becomes the visible book title and browser title automatically.

Recommended structure:

```md
# Book Title

## Chapter or major section

Normal prose paragraph.

### Subheading

More prose.
```

## Reader behaviour

The reader includes:

- runtime Markdown loading
- Marked parsing
- DOMPurify sanitisation
- browser-native text-to-speech
- Pakistani English preference when available
- click-anywhere-to-listen behaviour
- 1.05× default narration speed
- manual speed and voice controls
- pause / resume / stop
- reading and listening progress
- saved resume position
- a karaoke-style rolling word line beneath the active spoken paragraph
- responsive layout
- dark mode
- print rules

The browser progress key is isolated to this publication:

```text
imprecise-precis-progress-v1
```

## Hosting

The site is static and requires no package install, build command, server or database.

Once `manuscript.md` is added, the repository is ready to be published as a GitHub Pages reading room and wired into the TitanicParker Project Museum using the standard publication pattern.
