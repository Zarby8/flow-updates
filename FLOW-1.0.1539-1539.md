# FLOW 1.0.1539

**Coaches Notes print cleanly, page after page.** Two layout faults are fixed.
A section title could land on the last line of a page with its content overleaf,
so WEEKLY GOALS appeared at the foot of page one with the goals themselves on
page two — the title now moves to open the next page instead. And the frame that
performs that move was measuring from the wrong origin, which lowered the body's
bottom edge by 84 points and printed the tail of the notes straight through the
footer. Both are covered by tests that were checked in both directions: each one
fails when its fix is removed.

**GAME / OPPONENT reads like a name, not a filename.** A token stored as
AtlanticCoastAcademy16UNational now prints as Atlantic Coast Academy 16U
National.

**Wireless updates work again.** Every automatic update for the past week
downloaded correctly, verified its signature, and then failed to install with
"Update Backup Failed / Installation Postponed". FLOW's updater was routing the
install through a Sparkle helper built for sandboxed apps; FLOW has not been
sandboxed since September 6, so that helper could not replace the app in
Applications. FLOW now performs the install itself, the way a directly
distributed app should.
