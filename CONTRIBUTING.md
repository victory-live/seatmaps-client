<!-- This file is managed by Terraform (github-infra). Do not edit manually. -->
# Contributing

## Initial setup

After cloning, run the following to enable git hooks:

```sh
git config core.hooksPath .githooks
chmod +x .githooks/pre-commit .githooks/pre-push
```

This configures client-side hooks that prevent accidental commits and pushes
to protected branches (`main`, `main`).

## Workflow

1. Create a feature branch from the default branch
2. Make your changes and commit
3. Push your branch and open a pull request
4. Get code review approval (required)
5. Merge via the GitHub UI

```sh
git checkout -b my-feature-branch
# ... make changes ...
git add -A && git commit -m "Description of changes"
git push -u origin my-feature-branch
gh pr create
```

## Branch protection

Direct commits and pushes to protected branches are blocked by both
client-side git hooks and server-side GitHub rulesets. All changes must
go through pull requests with at least one approving review.
