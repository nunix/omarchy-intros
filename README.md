# omarchy-intros

Boot-intro videos for [Omarchy](https://omarchy.org/) — short clips that play
full-screen right after login, generated procedurally (no stock footage).
One directory per intro; see each one's own README for details and how it
was made.

- [`fire/`](fire/) — a "Hackers"-style burning OMARCHY wordmark
- [`zen-water/`](zen-water/) — gold-ink letters rising from ripples on dark
  water, timed to a short piano excerpt

## Install

```
omarchy-intro-install https://github.com/nunix/omarchy-intros.git <name>
```

e.g. `omarchy-intro-install https://github.com/nunix/omarchy-intros.git fire`.
This clones the repo, copies the named directory to
`~/.config/omarchy/intros/<name>/`, and sets it as the active boot-intro.
Pick between installed intros later from Omarchy's menu under
_Style > Boot Intro_, or `omarchy intro switcher`.

## Adding another intro

Add a new directory with an `intro.mp4` at its root (a `make-intro.py` and a
`README.md` are welcome, but not required), commit it, and install it with
the same command using that directory's name.
