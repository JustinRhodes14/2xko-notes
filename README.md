# 2XKO Notes

Personal fighting game notes page for 2XKO. Hosted on GitHub Pages.

## Adding / editing content

All notes live in `index.html` inside the `characters` object and `teamNotes` object near the top of the `<script>` tag. The comments in that section explain everything.

Quick reference:

| Thing to edit | Where |
|---|---|
| Combos | `characters.vi.combos` / `characters.thresh.combos` |
| Game plan | `characters.vi.gameplan` / etc. |
| Setups | `characters.vi.setups` / etc. |
| Knowledge / frame data | `characters.vi.knowledge` / etc. |
| Matchups | `characters.vi.matchups` / etc. |
| Team notes | `teamNotes` |
| Add a new character | Copy the template at the bottom of `characters` |

## Notation format

Write combos as a string where each token is separated by a space:

```
"5L > 2M > 5H > 214H"
"j.M > j.H > 5M > 5H > 236L"
"5M > 5H > [TAG] > 5M > 214H"
```

- **Directions**: numpad notation (1-9). `214` → ←↓↙, `236` → →↓↘
- **Buttons**: `L` `M` `H` `K` `A`
- **Combined**: `5L`, `2M`, `214H`, `j.H`
- **Separator**: `>`
- **Tag**: `[TAG]`

## Portrait images

Drop character portrait images into `assets/portraits/` and update the `portrait:` field:

```js
portrait: "assets/portraits/vi.png",
```

## Hosting on GitHub Pages

1. Push this repo to GitHub.
2. Go to Settings → Pages → Source → Deploy from branch → `main` / `root`.
3. Visit `https://yourusername.github.io/2xko-notes/`.
