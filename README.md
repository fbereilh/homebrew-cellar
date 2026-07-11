# homebrew-cellar

Homebrew tap for [Cellar](https://github.com/fbereilh/cellar) — an agent-first
notebook (a live Jupyter workspace with an MCP agent interface).

Cellar tracks **latest** (git `main`), not tagged releases, so it installs
`--HEAD`:

```sh
brew tap fbereilh/cellar
brew install --HEAD cellar          # or: brew install --HEAD fbereilh/cellar/cellar
```

> `fbereilh/cellar` is a **private** repo, so Homebrew clones `main` using your
> own GitHub git credentials (`gh auth`, SSH, or a PAT with repo access). Make
> sure you can `git clone git@github.com:fbereilh/cellar.git` first.

## Update

```sh
cellar --update                     # runs `brew update && brew upgrade --fetch-HEAD cellar`
```

`cellar --version` prints the version + build you are running.

The canonical copy of the formula lives in the app repo at
`packaging/homebrew/cellar.rb`; keep the two in sync.
