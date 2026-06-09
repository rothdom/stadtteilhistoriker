# stadtteilhistoriker.roth-dominik.de
Site in Hugo

- brew install hugo
- hugo server

## Types

- Posts: Normal Posts
- Wiki: Included in Top Menu Wiki Link
- Files: Shows all file attachments in Bundles & Included in Top Menu Link

## CI/CD and GitHub Actions

This repository builds and deploys itself with local GitHub Actions workflows:

- `hugo-builder.yml` builds the Hugo site and deploys it to GitHub Pages.
- `hugo-updater.yml` checks for new Hugo releases and updates `.hugoversion`.
- `dependabot-merger.yml` enables auto-merge for Dependabot pull requests.
