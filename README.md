# containerbase .github

![test](https://github.com/containerbase/.github/actions/workflows/test.yml/badge.svg)
![GitHub](https://img.shields.io/github/license/containerbase/.github)

This repository contains the basic containerbase configuration that is used in all other containerbase repositories.

## Development

`mise install` installs Node.js, pnpm, jactionlint, shellcheck, zizmor and the dependencies.

```bash
pnpm oxfmt           # pnpm oxfmt-fix to fix the formatting
jactionlint          # the GitHub workflows
zizmor .github/      # security audit of the GitHub workflows
```

CI runs jactionlint and zizmor through mise in the `lint` job, and the commit hook runs them on staged workflow files.
