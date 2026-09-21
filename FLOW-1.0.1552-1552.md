# FLOW 1.0.1552

**Updates no longer run a Mac out of memory.** Before installing an update,
FLOW backs up every project package. That backup read each game video in small
pieces but held on to every piece until the whole backup finished, so a Mac with
a dozen games climbed past 40 GB. macOS then paused FLOW, and Install and Relaunch
appeared to do nothing. The backup now frees each piece as soon as it is written,
so backing up a 1 GB video uses about 5 MB of memory instead of 3 GB.

Everything in 1.0.1550 is included: one-click SINCE LAST BREAKDOWN with BOB coaching
targets, a named message when the last breakdown is not in Brain yet, and Jev's
TEACHABLE NOW suggestions in COACHES NOTES.
