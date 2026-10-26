# Stagd

A live, seeded preview of your app for every pull request: built, started with its database and seed data, on a URL your team and reviewers can open. On your own compute (Namespace, Kubernetes, a Docker host), asleep when nobody uses it, gone with the pull request.

[stagd.dev](https://stagd.dev) · [app.stagd.dev](https://app.stagd.dev)

## Open source

- [**stagd**](https://github.com/stagdhq/stagd): the command line, `stagd relay` for compute Stagd can't reach, the Kubernetes manifests a cluster gets, and the API contract ([buf.build/stagdhq/stagd](https://buf.build/stagdhq/stagd)).
- [**homebrew-tap**](https://github.com/stagdhq/homebrew-tap): `brew install stagdhq/tap/stagd`.

```bash
curl -fsSL https://stagd.dev/install.sh | bash
```

Security issues: security@stagd.dev, privately.
