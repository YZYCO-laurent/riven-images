# riven-images

This repository is a static asset host for processed marketing images that need **direct public URLs** for external platforms such as Pinterest and Amazon.

## Folder system

Assets are organized by **client first**, then by **platform**.

| Path | Purpose |
|---|---|
| `clients/<client>/pinterest/` | Pinterest-ready assets |
| `clients/<client>/amazon/` | Amazon-ready assets |
| `clients/<client>/<platform>/` | Any future platform-specific assets |

A typical production path looks like this:

```text
clients/nmnlabo/pinterest/
clients/nmnlabo/amazon/
clients/another-brand/pinterest/
```

With GitHub Pages enabled, files will be reachable at URLs such as:

```text
https://yzyco-laurent.github.io/riven-images/clients/nmnlabo/pinterest/example.jpg
```

## Recommended conventions

Use lowercase folder names and hyphenated file names. Keep each rendered output file platform-specific so every public URL stays stable.

## Publishing

This repository includes a GitHub Actions workflow that deploys the repository contents to GitHub Pages whenever changes are pushed to `main`.
