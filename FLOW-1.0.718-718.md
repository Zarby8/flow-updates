# FLOW 1.0.718

This release hardens the core coaching workflow and prepares FLOW for daily production use.

- Loads the canonical GHOST client roster and keeps every client code window isolated by `ghost_id`.
- Creates exact-name timeline rows from code buttons with no predetermined lanes.
- Improves native video playback, fullscreen behavior, timeline reliability, package save/reopen, and real-media export.
- Adds durable Meeting Notes, IQ Library playback, BOB review, and client-scoped coaching context.
- Enforces owner-only local database and report storage.
- Limits reports to published ForceIQ coaching content and requires an explicit opponent for manual team scouting.
- Preserves transactional install backup and rollback support for Sparkle updates.

The ML models remain advisory and are not promoted by this release.
