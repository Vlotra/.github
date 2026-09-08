# Vlotra

We build [vlotpipe](https://github.com/Vlotra/vlotpipe) — a linter for CI pipelines, GitHub Actions and Azure Pipelines. It catches injection, credential, and supply-chain mistakes in your pipelines before they run, and is also a pipeline-aware YAML style linter — the half generic `yamllint` can't really do, since it has no notion of GitHub Actions or Azure Pipelines schema.

- **[vlotpipe](https://github.com/Vlotra/vlotpipe)** — the linter. `go install github.com/vlotra/vlotpipe/cmd/vlotpipe@latest`
- **[Try it online](https://vlotra.github.io/vlotpipe-site/playground/)** — no install, runs entirely in your browser via WebAssembly.
- **[Docs](https://vlotra.github.io/vlotpipe-site/docs/)**

Every rule is run against a real, actively-maintained pipeline — not just synthetic fixtures — before it ships, and every finding (and every *absence* of a finding) is verified against the actual source. See the [trophy case](https://github.com/Vlotra/vlotpipe/blob/master/docs/TROPHY_CASE.md) for the bugs that turned up along the way.
