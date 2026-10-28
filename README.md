# Sileo Repository (GitHub Pages)

A GitHub-only template for hosting an APT repository compatible with Sileo/Zebra.

## Setup from the GitHub website (no PC required)

1. Create a **public** GitHub repository named `repo` (or any name you prefer).
2. Upload the contents of this ZIP into the repository, keeping the `.github/workflows/` folder structure.
3. Upload your already-built `.deb` packages into the `debs/` folder.
4. Open **Settings → Pages** and set **Build and deployment → Source** to **GitHub Actions**.
5. Open **Actions** and run **Build Sileo Repository** (or push a commit to trigger it).
6. Once deployment succeeds, your source URL is:
   `https://YOURUSERNAME.github.io/REPONAME/`
7. Add that URL in Sileo → Sources → `+`.

## Important

- This repository hosts `.deb` packages; it does **not** build/compile tweaks.
- Put `.deb` files directly inside `debs/` (not in nested folders).
- Keep the workflow and folders in their current paths.
- The workflow fails clearly if no `.deb` packages are present.
- This is a basic unsigned APT repository template. For public distribution, review package compatibility and consider adding repository signing.
