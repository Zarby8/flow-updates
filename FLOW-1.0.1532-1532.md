# FLOW 1.0.1532

**A locked clip can be corrected.** Locking a clip into a client database was a
one-way door: the edit worked on screen, the clip never changed, and the fix died
with the window. It now lands, the header offers CORRECT CLIP beside the LOCKED
badge, and the commit button says what it does — UPDATE DATABASE CLIP. LOCK still
saves and advances in one step.

**The GAME REPORT eye stays green.** FLOW looked for a report by its template
name ("game_report") while Ghost titles the file with its human name
("… - Game Report - ….pdf"), so a report already saved in the package was
invisible and the eye greyed out until you asked for it again. Both sides are now
compared on the same folded key, so a report that exists — even offline — lights
the eye.

**QUICK DATABASE: tag a positive clip without leaving the timeline.** Select
the clip, press ⌘⇧P, and the DATABASE POSITIVES palette opens already on that
clip — the same palette, the same search, the same keys. ⌘↩ LOCK saves it,
confirms, and clears the window; you stay exactly where you were. The old
row-picker pass is untouched for batch work, and the hotkey is yours to change in
Settings > Shortcuts.

**Coaches Notes print with the breakdown, and look like ForceIQ.** The notes PDF
now rides the breakdown export into the client's game folder beside the movie,
carries the game rating you set in MEETING NOTES (and says UNRATED when there
isn't one, rather than inventing a number), and is rebuilt on the 2026 brand: the
real FORCE lightning lockup, black and white and gold, JetBrains Mono, page
numbers. The body no longer prints on top of its own header, the lockup is
upright, and GAME / OPPONENT / GAME DATE each get their own row.

**No tag you pick is ever dropped, and the palette speaks this season's
language.** Locking a clip used to write back only the tags the fuzzy matcher
happened to return — seven chosen tags could land as four, silently. Tag
resolution is now exact, anything outside the corpus is preserved rather than
discarded, and the palette refuses to close on a tag it cannot account for. The
bundled corpus is rebuilt from the current TAG export: PRESSURE READ (with SHOT
LANE), TECHNIQUE, O-ZONE, RUSH, BREAKOUT and GOAL LOCATION are all present.

**Wireless updates work again.** Every automatic update for the last week
downloaded correctly, verified its signature, and then failed to install with
"Update Backup Failed / Installation Postponed". The updater was routing the
install through a Sparkle helper built for sandboxed apps; FLOW has not been
sandboxed since September 6, so that helper could not replace the app in
Applications. FLOW now installs the update itself, the way a directly
distributed app should. This release must be installed by hand once; after that,
"Check for Updates…" works normally.
