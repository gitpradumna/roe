# Matrix Build Demo (build-4ad9098)

This repository contains a GitHub Actions workflow that demonstrates a multi-platform matrix build with artifact management.

## What the workflow does

- Runs a matrix across 3 OS runners and 3 Node.js versions (total 9 parallel jobs).
- Each matrix job runs a step named `matrix-4ad9098`.
- Each job generates a non-empty artifact file and uploads it using `actions/upload-artifact@v4`.
- Artifacts are named with the prefix `build-4ad9098-<variant>` (for example `build-4ad9098-ubuntu-latest-node14`).

## Files of interest

- `.github/workflows/matrix-build.yml` — the CI workflow definition.
- `README.md` — this file.

## Validation checklist

- At least 3 matrix jobs (the workflow uses 9 total).
- Each job uploads an artifact named `build-4ad9098-<variant>`.
- Each artifact contains non-empty content.
- The workflow includes a step named `matrix-4ad9098`.
- Make sure to push to `main` (or run manually via `workflow_dispatch`) and verify the Actions tab for successful runs and artifacts.

## Contact

If you need help integrating this workflow into your repository, email: **23f3002144@ds.study.iitm.ac.in**

