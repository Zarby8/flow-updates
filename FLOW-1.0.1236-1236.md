# FLOW 1.0.1236

- App Sandbox removed; container data migrates automatically on first launch (atomic, restorable, Release-isolatable), and now skips Realm sidecars, RealmCache, and non-regular files during migration.
- UAT candidate builds opt into test-mode isolation via the `FLOWAI_UAT_CANDIDATE` compile flag, keeping UAT runs off Chris's live data.
- FLOW-FEATURES conformance graph added, covering menu, shortcuts, import-service HTTP, Sparkle release, and `.flowaipkg` contract.
- App-target build fix after sandbox removal (migration entry point made public, dropped app-level `FlowLog` calls).
