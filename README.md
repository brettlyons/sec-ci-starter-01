![CI](https://github.com/brettlyons/secure-ci-starter/actions/workflows/security.yml/badge.svg)

# sec-ci-starter-01

Small demo of a security gate in CI using GitHub Actions.

## What it does
- Runs on every push / pull request
- Audits Python dependencies with `pip-audit`
- Fails the build if known vulnerable packages are detected

## How to reproduce
1. Edit `requirements.txt` to an old/vulnerable version (expect CI to fail)
2. Bump the dependency (expect CI to pass)

## Why ?
This is a minimal example of shifting security left by making risk visible at commit time.
