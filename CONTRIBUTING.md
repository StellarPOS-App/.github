# Contributing to StellarPOS

Thanks for your interest. These guidelines apply to every StellarPOS
repository. Each repository's own `CONTRIBUTING.md` adds setup steps and
conventions specific to it.

## Ways to help

- Fix a bug or build a feature from the open issues
- Improve tests, documentation, or accessibility
- Try StellarPOS in a real shop and tell us what got in the way
- Review open pull requests

## Workflow

1. **Find or open an issue first** for anything beyond a typo, and comment
   that you are taking it. This avoids duplicated work and lets the design
   be agreed early.
2. **Fork and branch** from `main`: `feat/<short-name>`, `fix/<short-name>`,
   `docs/<short-name>`.
3. **Commit** with [Conventional Commits](https://www.conventionalcommits.org/):
   `feat(pos): add receipt reprint`, `fix(payments): reject short payments`.
   Keep commits focused, so one commit does one thing.
4. **Run the checks** before pushing. Each repository has a single command
   (`npm run check` or `make check`) that runs what CI runs.
5. **Open a pull request** using the template. Explain the problem as well as
   the fix, describe how you tested it, and link issues with `Closes #N`.

## Standards

- **Tests come with changes.** New behavior needs tests, and bug fixes need a
  test that fails without the fix.
- **Money is never a float.** Use integer cents for store amounts and
  integer stroops for Stellar amounts.
- **Never handle secret keys.** StellarPOS is non-custodial by design. No
  change may make the backend or app receive, store, or log a Stellar secret
  key.
- **No secrets in code.** Configuration goes through environment variables,
  documented in `.env.example`.
- **Accessible by default.** Every control needs an accessible name and must
  work from the keyboard.
- **No emoji** in code, commit messages, issues, or docs. Keep the project's
  writing plain.

## Reviews

A maintainer reviews every pull request. Changes to payment verification,
authorization, or contract fund movement need two approvals.

## Conduct

Everyone participating agrees to the [Code of Conduct](CODE_OF_CONDUCT.md).
