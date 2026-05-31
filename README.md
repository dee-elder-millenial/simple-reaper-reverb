# Simple Reaper Reverb

A lightweight stereo reverb for [REAPER](https://www.reaper.fm/), packaged as a native JSFX effect.

Simple Reaper Reverb is intentionally small, dependency-free, and easy to inspect. It uses a compact Schroeder-style design: parallel feedback comb filters for the tail, simple damping in the feedback path, and all-pass stages for diffusion.

## Features

- Native REAPER JSFX plugin, no VST/AU build step required
- Stereo reverb with adjustable width
- Room size, damping, pre-delay, wet/dry mix, and output trim
- Plain-text source that can be copied, modified, and shared
- MIT licensed

## Download

Download the plugin file directly:

[Effects/Simple Reverb.jsfx](Effects/Simple%20Reverb.jsfx)

Or download the repository as a ZIP from GitHub:

`Code > Download ZIP`

## Install

1. In REAPER, choose `Options > Show REAPER resource path in explorer/finder`.
2. Open the `Effects` folder.
3. Copy `Effects/Simple Reverb.jsfx` into that folder.
4. In REAPER, open the FX browser.
5. Choose `FX > Scan for new plugins`.
6. Search for `Simple Reverb` under `JS`.

Important: JSFX files go in REAPER's `Effects` folder, not `UserPlugins`. `UserPlugins` is for REAPER extension binaries.

More detailed installation notes are in [INSTALL.md](INSTALL.md).

## Controls

| Control | What it does |
| --- | --- |
| `Room Size` | Increases the reverb tail length and apparent room scale. |
| `Damping` | Darkens the decay by rolling high frequencies out of the feedback path. |
| `Pre-delay` | Adds a gap before the reverb bloom. |
| `Wet` | Sets the reverb level. |
| `Dry` | Sets the original signal level. |
| `Width` | Adjusts the stereo spread of the reverb return. |
| `Output` | Final gain trim. |

## Development

The plugin is a single JSFX file:

`Effects/Simple Reverb.jsfx`

To edit it, change the file in your REAPER `Effects` folder or copy this repository version there after each edit. REAPER can reload JSFX from the FX window after rescanning or reopening the effect.

## License

MIT. See [LICENSE](LICENSE).
