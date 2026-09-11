# homebrew-bearing

Homebrew tap for [Bearing](https://github.com/moberghr/bearing) — a cross-platform SQL query tool and
script manager.

```bash
brew install --cask --no-quarantine moberghr/bearing/bearing
```

`--no-quarantine` is required while the app is unsigned: macOS otherwise reports "Bearing is damaged and
can't be opened", which is Gatekeeper refusing a quarantined ad-hoc-signed bundle, not a bad download.

Apple Silicon only. Bearing updates itself from its own GitHub Releases feed, so `brew upgrade` is not
part of the update path.

> `Casks/bearing.rb` is a **copy**. The canonical source lives in the app repo at
> [`packaging/homebrew/bearing.rb`](https://github.com/moberghr/bearing/blob/main/packaging/homebrew/bearing.rb);
> edit it there and copy it here. The per-release steps are in that directory's README.
