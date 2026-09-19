# Project setup

## First five minutes

1. Create a repository from `noerith-starter`, or clone/copy it if template creation is unavailable on the current GitHub plan.
2. Run `./scripts/initialize.sh` with the project name, description, and problem statement.
3. Record the first technical decision in `docs/decisions/`.
4. Run `./ci/verify.sh` locally and open a pull request.
5. Add the project ecosystem to `.github/dependabot.yml` once a package manager is selected.

## Security baseline

- Keep credentials outside Git history.
- Use GitHub environment secrets only when a deployment requires them.
- Keep CI permissions read-only unless a specific job needs a narrow write permission.
- Review major dependency updates manually.
- Report vulnerabilities through the organization security policy.

## GitHub Free boundaries

This starter does not rely on paid GitHub features. If branch or ruleset enforcement is unavailable for a private repository, use the documented pull-request workflow as the operating standard and record exceptions in the pull request.
