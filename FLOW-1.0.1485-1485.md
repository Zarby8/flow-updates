# FLOW 1.0.1485

**Updates install again.** FLOW refuses to hand off to Sparkle until it has
sealed a backup of the live database plus every project package, and that check
had a flaw: packages FLOW creates itself (Ghost SHIFTS imports, provider-media
intake, manual cuts) store an "app-owned" bookmark, and the backup asked for all
of them as if they were operator-chosen ones. A single such package therefore
refused the whole update on any machine that had ever imported one — the update
sat on *Installation Postponed* with no way forward. The check now accepts both
bookmark kinds, and if a package genuinely cannot be reopened it says so by name
and by cause instead of blaming the backup.

**The player line in clip text is just the player.** A clip's burned text used to
be able to read `#PLAYERNAME: #11 HENRY MEIER`. Editing a seeded `#PlayerName`
label stored the label's name as `#PlayerName: <the resolved value>`, and that
whole string then became part of the clip. The player row now renders the
identity alone — `#11 HENRY MEIER` — whether the prefix arrives through the
label's name or its value, and it keeps its place at the front of the LABELS
order. Clips already stamped that way read correctly; nothing on disk is
rewritten. The other three seeded rows keep their self-explanatory `TEAM:`,
`OPPONENT:` and `GAME DATE:` prefixes.
