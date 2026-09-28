# zen-water

A boot-intro video for [Omarchy](https://omarchy.org/): gold-ink letters of
OMARCHY rise one at a time from ripples on dark water, in a jade palette,
generated procedurally (no stock footage). Letter timing follows the actual
note onsets in the music, found via spectral-flux peak-picking, and the
visual fade-out is synced to the music's own fade so both end together.

Install:

```
omarchy-intro-install https://github.com/nunix/omarchy-intros.git zen-water
```

This clones the repo and copies this directory to
`~/.config/omarchy/intros/zen-water/`, then sets it as the active boot-intro.
Switch back to it later with:

```
intro=$(omarchy-intro-switcher); [[ -n $intro ]] && omarchy-intro-set "$intro"
```

or `omarchy-intro-set zen-water` directly.

## Audio

`mrlawrence-8s.wav` is an 8-second excerpt (0:56-1:04) of Ryuichi Sakamoto's
"Merry Christmas Mr. Lawrence", used here for a personal, non-commercial
desktop customization. It is not original work — if you fork this repo for
your own redistribution, swap it for audio you have the rights to use.

## Regenerating intro.mp4

```
uv run --with numpy --with pillow make-intro.py
```

Requires `ffmpeg`, `mrlawrence-8s.wav` alongside the script, and the
`JetBrainsMonoNerdFont-Bold` font.

## Pairs well with

Visually, this fits a dark, muted, natural-tone theme — e.g.
[Osaka Jade](https://omarchy.org/). This is just a suggestion for your own
theme; Omarchy boot-intros aren't tied to a specific theme.
