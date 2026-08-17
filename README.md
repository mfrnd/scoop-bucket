# scoop-bucket

Personal [Scoop](https://scoop.sh) bucket for my applications.

## Install

```powershell
scoop bucket add mfrnd https://github.com/mfrnd/scoop-bucket
scoop install <app>
```

Update everything later with `scoop update *`. Manifests are kept current
automatically by the daily [Excavator](.github/workflows/excavator.yml)
workflow, which tracks each app's latest release.

## Apps

### [sourcegit](https://github.com/mfrnd/sourcegit)

Personal fork of the SourceGit Git GUI, adding an optional Sourcetree-style
"uncommitted changes" row at the top of the history graph.

```powershell
scoop install sourcegit
```

## Adding an app

Drop a `bucket/<app>.json` manifest (with `checkver` + `autoupdate` pointing at
the app's GitHub releases) and add a short section for it above. Excavator picks
it up and keeps it updated automatically.
