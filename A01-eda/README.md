# A01 — Exploratory Data “Ping” (mini-EDA)

Goal: make one tiny, reproducible change to a plot and show it in `figs/`, then submit via an Issue.

## What you’ll do
- [ ] Change the **binning** of a histogram **or** pick a **different numeric column** to plot.
- [ ] Re-run the notebook/script so a **new PNG** appears in `A01-eda/figs/`.
- [ ] Commit with a **meaningful message** and **push**.
- [ ] Open an **Issue** titled **“A01 ready”** and paste your **latest commit hash**.

---

## Repo layout
```bash
A01-eda/
data/ # small CSVs
figs/ # your exported PNGs go here
notebooks/ # the notebook/script you run
README.md
```


## Step-by-step

1) **Open the notebook/script**
   - Use the starter in `A01-eda/notebooks/` (or create a small script).

2) **Make exactly one EDA change**
   - Example A: change `bins=30` → `bins=12`
   - Example B: switch from column `price` → `tip`
   - Keep everything else the same.

3) **Export the figure**
   - Ensure your code saves a PNG to `A01-eda/figs/` (e.g., `plt.savefig("../figs/hist_tip.png", dpi=150)`).

4) **Commit & push**
   ```bash
   git add -A A01-eda
   git commit -m "A01: update histogram (bins=12) and export PNG"
   git push

5) **Submit via Issue**

- **Get your latest commit hash:** run `git log --oneline -1` and copy the first 7 characters (e.g., `a1b2c3d`).
- **Open a new Issue** titled **A01 ready**.
- **Paste this in the body:**
  - **Latest commit:** `a1b2c3d`
  - **What changed:** one sentence (e.g., “Changed histogram bins to 12” or “Switched column to `tip`”)
  - **(Optional) PR link:** https://github.com/<owner>/<repo>/pull/<number>
