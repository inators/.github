# inators LLC

## Git Workflow

IMPORTANT: Never push directly to `main`. Always create a feature branch and open a PR. Org rulesets enforce this server-side, but respect the workflow locally too.

### Branch Naming

Branches must follow `username/type/description` format. Enforced by org ruleset.

- **username**: your GitHub username identifier
- **type**: `feat`, `fix`, `docs`, `chore`, `refactor`, `test`, `perf`, `ci`, `build`, `revert`
- **description**: kebab-case, lowercase, no uppercase

Examples: `zachthedev/feat/user-auth`, `claude/fix/login-race-condition`, `claude/ci/alls-green-gate`

## Git Commits

IMPORTANT: Never use `git commit` directly. Always use the `/commit` slash command for all commits. This ensures commits are GPG-signed with the correct key.

## Release Bot (`inators-release-bot`)

Release Please uses a custom GitHub App token (`inators-release-bot`, App ID `2819015`) instead of `GITHUB_TOKEN` so it can bypass the org tag protection ruleset to create `v*` tags.
