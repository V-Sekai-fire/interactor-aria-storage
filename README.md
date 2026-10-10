# interactor-aria-storage

An Elixir library for content-defined chunk storage that reads and writes the casync and desync chunk-store format.

## What it is for

It splits a file into content-defined chunks, stores each one compressed under its hash, and writes the index that reassembles the file, in the layout a desync store also reads. Chunks go to a local directory or to an object-storage backend. `lib/README.md` describes the modules.

## Build

```sh
mix deps.get
mix test
```

## Licence

MIT. See [LICENSE](LICENSE). The vendored desync source under `thirdparty/` keeps its own BSD-3-Clause licence.
