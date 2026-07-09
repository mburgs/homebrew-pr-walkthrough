# homebrew-pr-walkthrough

Homebrew tap — the **public distribution channel** for
[`pr-walkthrough`](https://github.com/mburgs/pr-walkthrough), whose
source repo is private.

## Install

```bash
brew install mburgs/pr-walkthrough/pr-walkthrough
```

## Update

```bash
brew upgrade pr-walkthrough
```

## How this works — do not hand-edit

`Formula/pr-walkthrough.rb` is **generated and force-pushed by CI** in
the private source repo on every merge to `main` (rolling releases).
The release tarball it points at is attached to a GitHub Release *in
this repo*. Manual edits will be overwritten on the next publish.

Requires macOS on Apple Silicon (arm64) — local STT runs on MLX, which
ships arm64-only wheels.
