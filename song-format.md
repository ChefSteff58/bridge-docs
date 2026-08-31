# The song file format

**The promise: you can read your songs without Bridge.** Every song exports as plain
text, in a format that predates every app in this category — and that any text editor,
on any computer, will still open in thirty years. Bridge's PDF export is the pretty
one; this is the durable one. Neither ever requires a subscription, a login, or the
app itself.

## The format

A exported song is a single UTF-8 plain-text file:

```
Golden Hour
Key of C · 96 BPM · capo 2

Chords
    C  x32010
    G  320003
   Am  x02210

Verse
C          G
Coffee in the morning light
Am
Steam against the window

Chorus
C  G  Am  F

Notes
Second verse still needs a bridge into the turn.
```

Reading it:

- **The first line** is the title. The second line lists only the facts the song has —
  key, tempo, capo — separated by " · ".
- **The Chords block** lists each chord the song uses with its fingering: six
  characters, low E string to high E, where `x` is muted, `0` is open, and a digit is
  the fret. Shapes above the 9th fret use dashes ("8-10-10-9-8-8").
- **Sections** (Verse, Chorus, …) are announced by their label on its own line. A line
  of chord names directly under the label is the section's progression.
- **Chords above lyrics**: a line of chord names aligned over the words they land on,
  in a monospaced column — the convention guitarists have traded songs in since long
  before smartphones. Open the file in any monospaced font and the chords sit over
  the right syllables.
- **Notes** at the end carries anything the writer kept with the song.

## Why this matters

Every songwriting app's reviews contain the same story: a subscription lapsed or a
company folded, and a catalog of songs went dark. Bridge is built so that story
cannot happen here. Export is never gated — not by the free tier, not by a lapsed
subscription — and the format above contains no Bridge-specific anything. Your songs
are yours, in a file your grandchildren's computers will open.
