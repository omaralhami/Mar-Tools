# Mar Tools — Public Downloads

Public release repository for Mar Tools desktop installers.

**Website:** [martools.net](https://martools.net)  
**Main development repo:** private / separate — this repo is **downloads only**.

## Releases

| Tool | Folder | Description |
|------|--------|-------------|
| SteaMar | [`releases/steamar/`](releases/steamar/) | Steam library utility |
| SpotiMar | [`releases/spotimar/`](releases/spotimar/) | Spotify client patcher (Windows) |
| MASMar | [`releases/masmar/`](releases/masmar/) | Windows licensing utility |

## File naming

Use the MSI filename from the Tauri build output, for example:

- `SteaMar_3.0.0_x64_en-US.msi`
- `SpotiMar_1.0.0_x64_en-US.msi`
- `MASMar_1.0.0_x64_en-US.msi`

Keep one **latest** copy per tool (overwrite on new release) or add versioned subfolders if you prefer history in git.

## Admin download URLs

Point Mar Tools website admin **Tool download links** at the raw GitHub URL for each MSI, for example:

```
https://github.com/omaralhami/Mar-Tools/raw/main/releases/steamar/SteaMar_3.0.0_x64_en-US.msi
```

Replace the path with the actual filename after you upload a build.

## Adding a release

1. Build the MSI from the tool’s Tauri project (`npm run tauri build` or your release script).
2. Copy the `.msi` into the matching folder under `releases/`.
3. Commit and push to `main`.
4. Update the download URL in the website admin panel if the filename changed.
