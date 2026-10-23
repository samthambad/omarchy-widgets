# Spreedy

A one-word speed reader for EPUB and plain-text books, in a 6x3 tile.

This is a fixed and extended copy of [cbarland's Spreedy](https://github.com/SimonSchubert/omarchy-widgets/tree/main/widgets/cbarland/spreedy)
(MIT). In the original, playback jumped straight to the end of every chunk because the
animation clock was compared against the Unix epoch; this version keeps Unix time in its own
source and only hands out a chunk when its deadline really passes.

What changed:

- Playback pauses while the page is off screen and picks up where it stopped.
- Controls that work by tap on the tile and a full-screen reader with four tabs:
  **Read** (large text), **Text** (a page around the current word, tap a word to jump),
  **Chapters** (EPUB table of contents, NCX or EPUB3) and **⚙** (speed, words at once,
  skip length, bookmarks, file).
- A bookmark per book, an end-of-book stop, and a position slider.
- "Words at once" (1-5) reads a phrase per flash; the clock still counts single words.
- Comes with Alice's Adventures in Wonderland, Chapter I, so it works without a file.
