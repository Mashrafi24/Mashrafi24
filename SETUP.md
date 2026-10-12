# Setup guide — Mashrafi24 GitHub profile

1. Create a **public** GitHub repository named exactly `Mashrafi24` under the `Mashrafi24` account, if it does not already exist.
2. Add the supplied `README.md` at the root and `.github/workflows/snake.yml` at the same paths shown in this package. Commit to `main`.
3. Go to repository **Settings → Actions → General → Workflow permissions** and allow **Read and write permissions** if available, then save. The workflow requires permission to push its `output` branch.
4. Go to **Actions → Generate contribution snake → Run workflow** (on `main`). Wait for success.
5. Confirm the `output` branch exists and contains `github-contribution-grid-snake-dark.svg`; refresh your GitHub profile. The workflow also runs daily and when its YAML is changed on `main`.
6. In your profile, use **Customize your pins** to select up to six of your best repositories. Start with the Java challenge, then prioritize larger completed projects.
7. Replace any project links or descriptions as your portfolio grows. If your default branch is not `main`, update `branches: [main]` in the workflow.

## Troubleshooting

- Snake missing: Check Actions run logs, repository workflow permissions, and the generated `output` branch. GitHub Actions might require enabling on a new repository.
- Stats unavailable: Those images depend on third-party services and can be rate limited. The rest of the README works independently.
- Profile README not visible: The repository must be public and have exactly the same name as your GitHub username, including capitalization.
- The `output` branch is generated content: do not manually edit it.
- GitHub scheduled workflows can be delayed, and inactivity can disable scheduled workflows. Manual dispatch remains available.

## Safety

No personal access token is required. This workflow uses the repository-scoped `GITHUB_TOKEN`. Review any third-party GitHub Actions before running them.
