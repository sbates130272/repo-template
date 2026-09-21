# repo-template

GitHub repository template with Stephen Bates' preferred CI defaults.

## What's included

- Secret scanning (gitleaks)
- Spellcheck on Markdown files
- ShellCheck on shell scripts
- GitHub Release workflow (tag-triggered)
- Label sync from `.github/labels.yml`
- PR template and issue templates (bug report, feature request)

## Using this template

```bash
gh repo create <owner>/<name> --template sbates130272/repo-template --clone
```

Or via the GitHub UI: click **Use this template** on the repo page.

## Post-creation checklist

- [ ] Update `README.md`
- [ ] Review `.github/workflows/*.yml` and delete any that don't apply (e.g. `shellcheck.yml` for non-shell projects)
- [ ] Adjust `.github/labels.yml` if needed and push to sync labels
- [ ] Add project-specific secrets in repo Settings → Secrets
- [ ] Set up branch protection (required status checks) in repo Settings → Branches
