# FLOW 1.0.1081

Built from `main` @ `5aa6f1ce` on 2026-09-02. Signed and notarized.

## What changed since 1.0.729

- IQ Library: period plays and pauses the preview without hovering; Tab and Shift-Tab step the selected set; PLAY SELECTED plays every selected clip once in visible order and stops at the last one; POSITION shows the SportsCode value; red action pills; alphabetical CLIENT menu.
- No transport key registers while a text field or a sheet owns input.
- Fullscreen clip-text overlay matches the in-window overlay at Retina density.
- Settings › DATABASES: root folder, one row per NHL database with CHOOSE / RESET, ADD DATABASE LOCATION for TAG-published season folders.
- Send to Breakdown: editable export name. Project identity chip reads `#21 NAME`. Organizer checkbox explained.
- Playback: media on /Volumes waits to keep up and reads 8 s ahead; stalls are logged for diagnosis.
- Database safety: a corrupt stored value no longer blocks startup; its bytes are quarantined, the value repaired, a pre-repair snapshot taken, and a rotating daily snapshot keeps a fresh restore point. The Ghost import edge now shares the app's database and listens on loopback only.
- Startup: cancellable 10 s restore with SKIP RESTORE; NHL reference databases enumerate and parse off the main thread; clip-write failures are surfaced; inverted clip ranges are rejected before persistence.

This update adds one database table (`persisted_json_quarantine`, created on demand) and changes no project package format. Signed build 1074 is retained for rollback.
