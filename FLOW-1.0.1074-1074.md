# FLOW 1.0.1074

Built from `main` @ `dd3304b1` on 2026-09-02. Signed, notarized, operator-verified.

## What changed since 1.0.729

- IQ Library: period plays and pauses the preview without hovering; Tab and Shift-Tab step the selected set; PLAY SELECTED plays every selected clip once in visible order and stops at the last one.
- No transport key registers while a text field or a sheet owns input.
- PLAYER panel shows POSITION from SportsCode UNGROUPED values; action strip pills are red; CLIENT menu is alphabetical.
- Fullscreen clip-text overlay matches the in-window overlay and renders at Retina density.
- Settings › DATABASES: root folder, one row per NHL database with CHOOSE / RESET, ADD DATABASE LOCATION for TAG-published season folders.
- Send to Breakdown: editable export name.
- Project identity chip reads `#21 NAME`; Organizer checkbox explained; Organizer scope label no longer reads as a selection count.
- Playback: media on /Volumes waits to keep up and reads 8 s ahead; local media unchanged.
- Startup: cancellable 10 s restore with SKIP RESTORE; NHL reference databases enumerate and parse off the main thread; window teardown of previews and hotkey monitors; clip-write failures are surfaced, never silent; inverted clip ranges are rejected before persistence.
