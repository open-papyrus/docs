# Contributing

## Prerequisites

- [git](https://git-scm.com/), [GitHub Desktop](https://desktop.github.com/), [GitKraken](https://www.gitkraken.com/git-client) or any other Git client
- some editor: [Visual Studio Code](https://code.visualstudio.com/)
- [rustup](https://rustup.rs/)
- [mdBook](https://rust-lang.github.io/mdBook/guide/installation.html): `cargo install mdbook`
- [mdbook-mermaid](https://github.com/badboy/mdbook-mermaid): `cargo install mdbook-mermaid`

## Editing

Open a terminal and start `mdbook`:

```bash
mdbook serve --open
```

This will open your browser, and you can start editing the files in [src](./src/).

## Committing

Before committing any changes, make sure to sign your commits using either [SSH](https://docs.github.com/en/authentication/managing-commit-signature-verification/about-commit-signature-verification#ssh-commit-signature-verification) (recommended) or [GPG](https://docs.github.com/en/authentication/managing-commit-signature-verification/about-commit-signature-verification#gpg-commit-signature-verification) commit signature verification. The master branch has branch protection rules in place and requires signed commits.
