# FLOW 1.0.1359
- Playback: forward slow-motion (0.25×–0.75×) is native AVPlayer rate again on every surface; reverse stays on the vsync chase clock. Measured on HEVC 1080p60 reels: 90/90 frames delivered vs 82/90 on the 1340 chase clock (#95)
- Reports: GAME REPORT fetches Ghost's auto-generated per-game PDF into `<Project>.flowaipkg/Reports/`, opens it in a new in-app PDF viewer; green EYE buttons under GAME REPORT and SINCE LAST BREAKDOWN reopen the latest; DOWNLOAD TO DESKTOP copies to `~/Desktop/FLOW/Reports/<Client>/`; report errors now surface as toasts (#97)
- SINCE LAST BREAKDOWN: SAVE PDF wired to Ghost's `since_last_breakdown` template (live when Ghost next deploys); the pulse shows in the viewer meanwhile (#97)
- BOB: instant read of any open report inside FLOW, with follow-up questions, over the existing BOB stream (#98, wiring PR)
- MEETING NOTES opens in its own window (no scrolling); hotkey settable in Settings → Hotkeys (default ⌘⇧D) (#96, #99)
- CLIP NOTES: Return commits the note and resumes playback; Shift/Option+Return inserts a newline (#96, #99)
