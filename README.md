# scoop-bucket

[Scoop](https://scoop.sh/) bucket for [Atlas Kaisar](https://github.com/AyoubTadlaoui)'s tools.

## Install

```powershell
scoop bucket add atlas https://github.com/AyoubTadlaoui/scoop-bucket
scoop install logx
```

Or one-liner:

```powershell
scoop install https://github.com/AyoubTadlaoui/scoop-bucket/raw/main/bucket/logx.json
```

## Available apps

| App | Project | Description |
|---|---|---|
| [`logx`](bucket/logx.json) | [GoLogX](https://github.com/AyoubTadlaoui/GoLogX) | Pretty-print JSON `slog` logs from stdin, files, or follow mode. |

## How updates land

For each tagged release of the upstream project, [goreleaser](https://goreleaser.com/) regenerates the manifest file with the new version + SHA256s and pushes the change here. The first manifest of each app may be hand-committed; subsequent releases are automated.

## License

Each app inherits the license of its upstream project. Most are MIT.
