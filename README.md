# [tinytype](https://hrhrprasath.github.io/tinytype) 

> A gentle typing game for toddlers — press keys, watch letters appear. No ads, no flash.



A gentle, screen-friendly typing game for toddlers. Press any letter or number — it appears center-screen with a soft pop, then settles into a growing numbered line at the top. No ads, no tracking, no flashy distractions.

Built as a single HTML file. Works on any device with a keyboard. Host it on GitHub Pages and share the link.

## Play

https://hrhrprasath.github.io/tinytype

## How it works

- **Letters & numbers** appear at center with a gentle pop animation, then float into a numbered line at the top.
- **Enter** starts a new line.
- **Backspace** removes the last character.
- **Auto word wrap** — when a line fills up, it wraps to the next line automatically.
- **Auto scroll** — the page follows along as lines grow.
- **Built-in timer** (default 3 min) — when it runs out, no more keys register. Shows a count at the end.
- **Soft synth sounds** — each key plays a gentle sine tone (different pitch per character). No audio files needed.

## Case selector

Three buttons at the top-right corner:

| Button | Behaviour |
|--------|-----------|
| **A**  | Always uppercase (default) |
| **a**  | Always lowercase |
| **Aa** | Keep case as typed |

## Timer

Default is 3 minutes. Customize via URL query parameter:

```
?time=2m    → 2 minutes
?time=30s   → 30 seconds
?time=120   → 120 seconds
```

## Design thoughts

Most "toddler apps" are overstimulating — bright flashing colours, loud sounds, aggressive animations. tinytype is the opposite.

**Pitch-black background** — reduces eye strain and ambient light in dark rooms. The screen blends into its surroundings.

**Muted colour palette** — 10 earthy, desaturated tones (sage, mauve, clay, teal). No pure reds or neons.

**Slow animations** — the pop-in takes 500ms, the float to position takes 1.3s. Nothing happens faster than a child can follow.

**No rewards, no scores** — the joy is in the cause-and-effect: press a key → something appears. The timer count at the end is just a number, not a judgement.

**Full keyboard takeover** — all browser shortcuts are suppressed so a toddler mashing keys won't accidentally close the tab or open developer tools. Only Escape works (to exit fullscreen).

**No external dependencies** — a single HTML file. No fonts to load, no CDN, no analytics, no third-party requests. Works offline once loaded.

**Synthetic audio** — the typing sounds are generated with the Web Audio API. Simple sine waves with quick decay — pleasant, non-copyrightable, no audio file needed.

## Deploy

This is a GitHub Pages–ready project. The only required file is `index.html` in the root.

1. Create a repository on GitHub named `tinytype`
2. Push the files (or just drag `index.html` into the repo on github.com)
3. Go to **Settings → Pages** and select `Deploy from a branch: main, / (root)`
4. Your game will be live at `https://your-username.github.io/tinytype`

No build step. No configuration.

## Contributing

Ideas and PRs welcome — open an issue to discuss before making changes.

## License

MIT

---

Powered by [OpenCode](https://opencode.ai)
