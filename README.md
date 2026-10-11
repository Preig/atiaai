# atiaai: The Fairbanks Prompt Kit, ATIA edition

Public URL: https://preig.github.io/atiaai/ (the QR codes on the annex slides point here).

## What it is

A single, self-contained web page (`index.html`) for Alaska tourism operators, from the session "Small Business Focus: Leveraging AI Solutions" (Pascual Reig-Munoz, Alaska SBDC) at the ATIA 2026 Annual Convention, Wednesday, October 14, 2026, Wedgewood Resort, Fairbanks.

It holds the hands-on workshop material:

- a context block people fill in once (saved only in their own browser) and put in front of every prompt;
- the 3-prompt build: a draft staff procedure, "three things wrong", and a stress test, with the 8-job menu;
- a pointer to the two ready-made assistants (Staff Procedure Coach and Campaign Builder) at https://preig.github.io/atiakit/team/;
- seven more prompts (translations, review replies, what AI says about you, alt text, agreements, job posts, training quiz);
- "What never goes in the box", "The real numbers", tools and FAQ, next steps and sources, with every obligation labeled Legal mandate, Contractual, Policy choice or Recommendation;
- companion links to https://preig.github.io/atiakit/ (with its Prompt-Kit-3x3.html and team/ pages) and https://preig.github.io/atiafuture/.

No external scripts, fonts, images or analytics: the logo is embedded in the file, and the page works offline once loaded. It sends nothing anywhere. The page carries `<meta name="robots" content="noindex">`, so search engines will not list it; remove that line if you want it found by search.

## How to publish (GitHub Pages)

1. Create a public repository named `atiaai` under the `preig` account.
2. Put `index.html` and the empty `.nojekyll` file (and this README if you like) at the root of the `main` branch. `.nojekyll` tells GitHub to serve the files as they are, without running its Jekyll site builder over them. In File Explorer it only shows when hidden files are visible.
3. In the repository: Settings > Pages > Build and deployment > Source: "Deploy from a branch". Branch: `main`, folder: `/ (root)`. Save.
4. Wait for the Pages build (a minute or two), then open https://preig.github.io/atiaai/ on a phone and a laptop. Check that the copy buttons work and that the context block is still there after a reload.
5. Scan the annex QR codes with a phone and confirm they open this page.

Command-line equivalent, from this folder:

```
git init -b main
git add index.html README.md .nojekyll
git commit -m "Publish the Fairbanks Prompt Kit, ATIA edition"
git remote add origin https://github.com/preig/atiaai.git
git push -u origin main
```

Then enable Pages as in step 3.

When to publish is your call (Policy choice). The earlier plan was to publish on the morning of the session; until it is published, the annex QR codes lead to a 404 page.

## Before you publish

- Re-read "The real numbers" against your current sources.
- Check that the companion links open (the atiakit and atiafuture sites need to be live).
- Open the page at phone and desktop widths, in light and dark mode.

## Editing

Edit `index.html` directly. Keep the rules used across the session materials: no em dashes or en dashes, no AI model version numbers, a label on every obligation, fictional data only in examples, and every prompt asks for its output to be marked DRAFT - PENDING OWNER REVIEW (the "what does AI say about you" check is the exception: its answer is evidence, not a draft). If you change the context block template in the script at the bottom of the page, people who already saved their own block keep theirs (it lives in their browser under the key `atia26.contextblock`).
