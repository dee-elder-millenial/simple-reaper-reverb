# Contributing

Contributions are welcome.

## Good changes to propose

- Clear bug fixes
- Better default settings
- Reverb quality improvements that keep CPU use modest
- Documentation fixes
- Preset suggestions

## Development notes

This project is intentionally simple. The main plugin lives in:

```text
Effects/Simple Reverb.jsfx
```

Please keep the plugin dependency-free and readable. If a DSP change is subtle, include a short note explaining what changed and why.

## Testing

Before proposing changes:

1. Copy the JSFX file into REAPER's `Effects` folder.
2. Rescan plugins or restart REAPER.
3. Load `Simple Reverb` on a track.
4. Check that all sliders respond smoothly.
5. Test with short percussive audio and sustained audio.
6. Listen for clicks, runaway feedback, silence, and clipping.

## Pull requests

Please include:

- A short summary of the change
- Any listening or compatibility notes
- Screenshots only if the change affects visible plugin UI
