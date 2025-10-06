# opim5512-a01-starter
This is the starter repo for A01 - where you will update the bins, change a variable to plot in the scatterplot, and update the README.md

## How does the auto-grader work?
## A01 Autograder — What It Checks

1. **PNG exists in `A01-eda/figs/`**
   - Fails with a clear message if no PNG is there.
   - Succeeds and prints a list of found PNGs when present.

2. **A figure changed in this PR** (compared to `main`)
   - Looks for changed files matching `A01-eda/figs/*.(png|jpg|jpeg)` using a three-dot diff `origin/main...HEAD`.
   - If none changed, it shows which files *did* change and tells you to re-save the figure.

3. **README updated**
   - Searches `A01-eda/README.md` for any of: `result`, `figure`, `summary`, `bins`, `hist`, `png`.
   - If none match, the grader asks for a 1–2 sentence note describing your change.

### How to get ✅ 10/10
- Change the histogram **bins** or pick a different **numeric column**.
- Re-run and **save a PNG** into `A01-eda/figs/`.
- Add a short note to `A01-eda/README.md` (one sentence is fine).
- Commit, push on a branch, and open a **Pull Request** to `main`.
