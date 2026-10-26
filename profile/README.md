# Stagd

A live, seeded preview of your app for every pull request: built, started with its database and seed data, on a URL your team and reviewers can open. On your own compute (Namespace, Kubernetes, a Docker host), asleep when nobody uses it, gone with the pull request.

[stagd.dev](https://stagd.dev) · [app.stagd.dev](https://app.stagd.dev)

## Open source

- [**stagd**](https://github.com/stagdhq/stagd): the command line, `stagd relay` for compute Stagd can't reach, the Kubernetes manifests a cluster gets, and the API contract ([buf.build/stagdhq/stagd](https://buf.build/stagdhq/stagd)).
- [**homebrew-tap**](https://github.com/stagdhq/homebrew-tap): `brew install stagdhq/tap/stagd`.

## Install the CLI

**macOS**, with Homebrew:

```bash
brew install stagdhq/tap/stagd
```

or without it: `curl -fsSL https://stagd.dev/install.sh | bash`.

**Linux**, any distribution (Debian, Ubuntu, Fedora, Arch, Alpine and the rest: the binary has no dependencies), on amd64 or arm64:

```bash
curl -fsSL https://stagd.dev/install.sh | bash
```

It checks the download against the release's checksums and puts `stagd` in `~/.local/bin`; `STAGD_INSTALL_DIR` for elsewhere, `STAGD_VERSION` for a given release. Homebrew on Linux works too.

**Windows**, on amd64 or arm64, in PowerShell:

```powershell
irm https://stagd.dev/install.ps1 | iex
```

It puts `stagd.exe` in `%LOCALAPPDATA%\Programs\stagd` and adds that to your PATH. In WSL, the Linux way above works too.

**With Go**, anywhere: `go install github.com/stagdhq/stagd/cmd/stagd@latest`.

Then `stagd login`. `stagd update` updates it; with Homebrew, `brew upgrade stagdhq/tap/stagd`, or `brew trust stagdhq/tap` once so a plain `brew upgrade` includes it (Homebrew 6 and later leaves untrusted taps out). What changed is in the [releases](https://github.com/stagdhq/stagd/releases).

Security issues: security@stagd.dev, privately.
