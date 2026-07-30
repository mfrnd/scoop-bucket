# scoop-bucket

Personal [Scoop](https://scoop.sh) bucket for the
[mfrnd/sourcegit](https://github.com/mfrnd/sourcegit) fork (SourceGit with the
optional "uncommitted changes in history" feature).

## Install

```powershell
scoop bucket add mfrnd https://github.com/mfrnd/scoop-bucket
scoop install sourcegit
```

Creates a `sourcegit` shim and a **SourceGit (fork)** Start-menu shortcut.

## Update

```powershell
scoop update sourcegit    # or: scoop update *
```

The manifest is kept current automatically by the daily **Excavator** workflow,
which tracks the fork's latest release and commits the new version + hashes.
