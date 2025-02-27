# stadtteilhistoriker.roth-dominik.de
Site in Hugo

- brew install hugo
- hugo server

## Types

- Posts: Normal Posts
- Wiki: Included in Top Menu Wiki Link
- Files: Shows all file attachments in Bundles & Included in Top Menu Link


## CI/CD and GitHub Actions

### Pushing Changes
- GitHub Actions builds and deploys the site when changes are pushed to main
- Uses peaceiris/actions-hugo@v3 for Hugo setup
- Build process optimized for consistency and reliability

### Dependabot & Auto-Merge
- **Dependabot**: Automatically updates GitHub Actions dependencies with daily checks
- Configured to group all GitHub Actions updates into a single PR
-  Using GitHub's recommended best practices with `dependabot/fetch-metadata` to safely auto-merge

### Hugo Updates
- `.hugoversion`: Contains the Hugo version used by GitHub Actions
- Custom Action: Checks weekly for new Hugo versions and creates PRs
- Direct auto-merge implementation in the update-hugo workflow
