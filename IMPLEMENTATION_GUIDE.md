# Implementation guide

Target repository: `SrujanRanganath/SrujanRanganath` (default branch `main`).

## 1. Copy the files in

Upload the contents of this package while preserving this structure:

```text
README.md
assets/                      (17 SVG files)
.github/workflows/snake.yml
IMPLEMENTATION_GUIDE.md
VALIDATION_REPORT.md
```

The README already references the SVGs using `assets/...` paths. Do not move the files out of that folder, and do not wrap README.md in extra code fences.

## 2. Allow the workflow to write

Repository Settings > Actions > General > Workflow permissions > select **Read and write permissions** > Save.

The workflow declares `contents: write`, but the repository setting must not block it.

## 3. Commit and push

Commit the README, `assets/` directory, and `.github/workflows/snake.yml` to `main`.

## 4. Confirm the snake exists

1. Open the Actions tab > "Generate contribution snake". Wait for a green run.
2. Check that an `output` branch now exists with these two files:
   - `github-contribution-grid-snake.svg`
   - `github-contribution-grid-snake-dark.svg`
3. If the run did not start, use Actions > Generate contribution snake > Run workflow.
4. Hard refresh your profile (Ctrl+Shift+R). GitHub may cache images briefly.

Until the first workflow run succeeds, the snake image will be unavailable. The rest of the README uses local SVG assets.

## 5. Verify featured repositories

Open each project button while logged out or in a private window. The AI Engineering Workspace repository was not publicly accessible during the prior inspection; confirm it is public and that its URL is correct before featuring it to recruiters.

## 6. Final checks

- Open the LeetCode card URL in a browser; if the card fails, the direct profile button remains available.
- Confirm skill icon rendering; the `skillicons.dev` service is external.
- Review the skill tiers and adjust them to match your actual experience.
- Consider cleaning the Striver DSA repository's committed `.exe` files and failing workflow before directing recruiters there.
