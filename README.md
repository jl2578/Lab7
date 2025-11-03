# Lab 7 — One-Sample t-Tests & Confidence Intervals (DSARM 1)

This repository is Codespaces‑ready and mirrors the setup of earlier labs, providing a reproducible environment for completing the Lab 7 notebook.  Lab 7 focuses on hypothesis testing for a single mean in public policy and health contexts.  You will learn to perform **one-sample *t*-tests**, calculate and interpret **confidence intervals**, and compute **Cohen’s d** effect sizes using the synthetic behavioral health dataset.

## Contents

- **Lab7.ipynb** — notebook guiding you through one-sample *t*-tests, confidence intervals, and effect size calculations.
- **ABCD_synthetic.csv** — synthetic behavioral health dataset for Lab 7.
- **figures/** — export your images here (ignored by Git; includes `.gitkeep`).
- **.devcontainer/** — dev container definition used by GitHub Codespaces to preinstall dependencies and useful VS Code extensions.
- **requirements.txt** — Python requirements for a lightweight scientific stack.
- **.gitattributes** — configures `nbstripout` to keep notebook diffs clean.
- **.gitignore** — ignores temporary files, OS clutter, and the `figures/` folder.
- **LICENSE** — CC0‑1.0 license notice.

## Quick start (GitHub Codespaces)

1. Click **“Open in GitHub Codespaces”** or use **Code → Create codespace on `main`**.  The Codespace will build using the provided dev container; dependencies install automatically via `requirements.txt`, and `nbstripout` is installed to keep notebook diffs clean.
2. Once your Codespace is ready, open `Lab7.ipynb` and run all cells in order (`Kernel → Restart & Run All`) to avoid hidden state.
3. Save any plots or output figures to the `figures/` folder using code like:

   ```python
   plt.savefig("figures/hist_mean.png", dpi=150, bbox_inches="tight")
   ```

4. Use VS Code’s **Data Wrangler** (`Command Palette → "Launch Data Wrangler"`) to inspect and clean the dataset if needed.

### Saving your work

Codespaces auto‑saves changes in the workspace, but they are **not** synced to GitHub until you commit and push.  To persist your work:

- Use the **Source Control** view to commit changes with a message.
- Click **Sync** or run `git push` to push the commit to GitHub.
- Consider exporting key figures or PDFs as an extra backup.

Inactive Codespaces may be deleted after 30 days.  Commit and push regularly to avoid losing work.

## Reproducibility & good practices

- Always run notebook cells in order.  If you restart the kernel, run all cells again.
- Save plots to the `figures/` folder.  The folder is ignored by Git to keep history slim.  The `.gitkeep` file ensures the folder exists.
- To enforce clean notebook diffs locally outside Codespaces, install `nbstripout` and run `nbstripout --install` in the repository (the dev container does this automatically).
- Use `pip install -r requirements.txt` in other environments to install dependencies.

## Troubleshooting

- **`ModuleNotFoundError`**:  Run `pip install -r requirements.txt` in the active environment.
- **`FileNotFoundError: figures/...`**:  Ensure the `figures/` directory exists, e.g. `os.makedirs("figures", exist_ok=True)`.
- **Changes not persisting**:  Commit and push; Codespaces can be temporary.

## License

This work is released under the CC0 1.0 Universal public domain dedication.  See `LICENSE` for details.
