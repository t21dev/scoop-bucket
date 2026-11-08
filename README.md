# t21dev Scoop bucket

Scoop manifests for apps by [t21 dev](https://t21.dev).

```powershell
scoop bucket add t21dev https://github.com/t21dev/scoop-bucket
scoop install t21dev/turbo-reader
scoop install t21dev/porter
scoop install t21dev/dev-cleaner
scoop install t21dev/kitab
```

| App | What it is |
| --- | --- |
| `turbo-reader` | [Turbo Reader](https://turbo-reader.t21.dev), a fast, small RSS reader. Adds a `turbo-reader` command, so `turbo-reader --mcp` works for AI agents. |
| `kitab` | [Kitab Reader](https://github.com/t21dev/kitab), a fast, native reader for PDF, ebooks and Markdown. Adds a `kitab` command. |
| `porter` | [Porter](https://porter.t21.dev), see which process holds a port and stop it. |
| `dev-cleaner` | [Dev Cleaner](https://github.com/TriptoAfsin/dev-cleaner), reclaim disk and memory from developer caches, build folders, AI models and ports. Runs portable; settings persist across updates. |

Each installs from the portable zip. Your library, settings and pinned ports
live in `~\scoop\persist\<app>\data` and survive updates.

## Updates

`.github/workflows/excavator.yml` checks for new GitHub releases every hour
and commits the new version, URL and hash.
