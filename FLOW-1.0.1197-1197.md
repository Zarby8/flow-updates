# FLOW 1.0.1197

- ⌘K command palette with the Feature Map and the Highlights workflow: mark a selected video-lane clip with H, persist Highlights as a client-DB tag, and jump to live workflows from the palette.
- Ghost shift handoff receipts now identify the FLOW service correctly, so Alumni/handoff packages no longer 409 on delivery.
- FLOW Import Edge runtime works for either owner (Chris or Shane); the installer no longer ad-hoc signs and strips quarantine after install (FLOW-INST-01).
- Accessibility fixes for the clip strip: per-clip targets, hosted clip AX walked via NSView, and the AX tree walk that could crash on CI removed.
- Playback and library fixes: black-frame detection, IQ Library recenter, HANDEDNESS ordering, seek tolerance, container-local bookmarks, and font registration fallback.
- BOB cockpit responses are structured and streaming updates are coalesced; NHL provider clocks are kept out of authored notes.
