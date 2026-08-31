# QV

The site of Queres Viver. Two pages, `index.html` and `sobre.html`, served by
GitHub Pages at `queresviver.pt`. No build step.

## Commit identity

Commit as `QV <queresvivere@proton.me>`:

    git config user.name "QV"
    git config user.email "queresvivere@proton.me"

This lives in `.git/config`, which no clone carries, so set it before the first
commit of a session and check `git log -1 --format='%ae'` before pushing. The
history was rewritten once to take a personal address back out of all 45
commits; nothing should put one in again.

## House rules

- **No JavaScript.** The language switcher on `sobre.html` is `:target`, and
  the default state is `:has()`. Keep it that way.
- **CSS only where it does a job.** Every rule in either `<style>` block is
  there for a stated reason and carries a comment saying which. Naked HTML is
  the design: browser defaults, blue links, Times New Roman. This was chosen
  deliberately and is not an oversight to correct.
- **Never describe QV as "crítica cultural"** or invent a description for it.
  Where a description is needed — meta tags, JSON-LD, Open Graph — use QV's own
  statement, verbatim, as it already appears in `index.html`.
- **Do not invent words.** In the translations on `sobre.html`, a real
  borrowing is right and a plausible-sounding construction is not. If a
  language has no word for it, leave the language out.
- Texts run newest first, each an `<article>` with its own `id`, and the record
  sentence sits above the title.
