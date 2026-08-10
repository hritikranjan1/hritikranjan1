# Hritik Ranjan — GitHub Profile Setup

## 1. Create the profile repository

Create a **public** repository named exactly:

`hritikranjan1`

This is GitHub's special profile repository.

## 2. Copy these files

Copy:
- `README.md` -> repository root
- `assets/dark.svg` -> `assets/dark.svg`
- `assets/light.svg` -> `assets/light.svg`
- `.github/workflows/snake.yml` -> `.github/workflows/snake.yml`

## 3. Enable GitHub Actions write permission

Repository:
Settings -> Actions -> General -> Workflow permissions -> **Read and write permissions** -> Save.

## 4. Run the Snake workflow

Open:
Actions -> Generate Snake Animation -> Run workflow

Wait for the first green run. It creates the `output` branch.

## 5. Self-host GitHub stats

Follow the supplied setup guide:
- Create a GitHub classic PAT with `repo` scope.
- Fork `anuraghazra/github-readme-stats`.
- Deploy the fork to Vercel Hobby.
- Add Vercel environment variable `PAT_1`.
- Copy the generated Vercel instance URL.
- In `README.md`, replace both `YOUR-INSTANCE.vercel.app` occurrences.

Never put the PAT in README, GitHub code, or chat.

## 6. Verify

Switch GitHub between dark/light appearance and reload the profile.
The banner and contribution snake should change with the theme.

## Important

The animated banner in this package is self-contained SVG. The three logo moments are compact visual marks/labels because no external logo reference files were supplied. If you provide official Playwright/AWS/Kubernetes logo reference images later, the banner can be refined to trace those exact references.
