# Security Policy

StellarPOS handles payments, so we take security reports seriously.

## Reporting a vulnerability

Report privately through GitHub's private vulnerability reporting on the
affected repository:

- [surface](https://github.com/StellarPOS-App/surface/security/advisories/new): the point-of-sale app
- [backend](https://github.com/StellarPOS-App/backend/security/advisories/new): API and payment verification
- [contracts](https://github.com/StellarPOS-App/contracts/security/advisories/new): Soroban contracts

Do **not** open a public issue, pull request, or discussion about a
vulnerability.

Include what you found, its impact, and steps to reproduce. A failing test is
ideal. We aim to acknowledge reports within 3 business days and to agree a
disclosure date with you before anything is made public.

Each repository's own `SECURITY.md` lists what is in scope there and the
security properties we rely on.

## Supported versions

Only the latest `main` of each repository receives security fixes. The
contracts have not been externally audited yet.
