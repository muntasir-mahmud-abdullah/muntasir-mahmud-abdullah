# Setup: Muntasir's GitHub Profile README

## Files

- `README.md` — profile README for `muntasir-mahmud-abdullah/muntasir-mahmud-abdullah`
- `assets/github-banner.svg` — custom banner used at the top of the README
- `.github/workflows/snake.yml` — GitHub Actions workflow that generates the contribution-snake SVGs

## Publish the profile README

1. Open the repository `https://github.com/muntasir-mahmud-abdullah/muntasir-mahmud-abdullah`.
2. Replace its root `README.md` with this package's `README.md`.
3. Upload the `assets/` directory, preserving the `assets/github-banner.svg` path.
4. Upload `.github/workflows/snake.yml`, preserving the directory structure.
5. Commit the files to the repository's default branch.

## Enable the contribution snake

- Ensure GitHub Actions is enabled for the profile repository.
- The workflow currently runs on pushes to `main`, on a daily schedule, and manually through `workflow_dispatch`.
- If the repository's default branch is not `main`, change the branch under the workflow's `push.branches` setting.
- After the first successful workflow run, GitHub Actions creates/updates the `output` branch. The snake images in the README will then load from that branch.
- The workflow needs repository contents write permission. The workflow file declares `permissions: contents: write`; check the repository's Actions settings if the workflow cannot push.

## Notes

- The README uses external image services for technology icons, typing SVG, stats, streaks, and the profile-view counter. These services must be reachable for the images to display.
- GitHub language statistics describe repository language composition; they are not a measurement of professional proficiency.
- The banner references your public GitHub avatar. The `MM` monogram in the SVG is the fallback if the external avatar image is not rendered by a viewer.
- Review public profile visibility and contact details before publishing. The README intentionally uses city-level location only.
