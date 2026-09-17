# FLOW 1.0.1507

**Breakdowns stop failing on the last second of a clip.** A Teaching Point row
failed with *"FLOW could not read the source video"* while the Positives row kept
rendering, and RETRY did the same thing. A freeze-and-draw hold inside the last
second of the game video asked FLOW for a full second of frames that did not
exist past the end of the file, and AVFoundation refused the entire row. A hold
at the very end now freezes on the last real frame, and a range that genuinely
holds no frames now names the range and how long the source is instead of
answering with a number.

**Database clips are about six times smaller.** Locking a clip into a client
database re-encoded it at the near-lossless rate a telestration burn needs —
1920x1080x60 at 1.0 bits per pixel, about 125 Mbps — even though a database clip
is a plain in/out of footage that is already encoded. On Chris's library that was
7.28 GB for 44 clips: 165 MB on average, and 302 MB for a single 19-second clip.
A clip with nothing burned into it is now copied bit-for-bit, and a clip that
does need a re-encode is capped at 20 Mbps. Worth noting what does not change:
the archived media, the clip's timing, its tags, and its playability from IQ
Library are all exactly as before — only the bytes on disk get honest.

**Updates install again on a machine that has forgotten packages.** FLOW
remembers where your packages live so the install-time backup can prove it has
everything before it installs an update. Two remembered packages that were gone
from disk — one deleted, one renamed — made every update postpone with *"a
remembered package could not be reopened,"* and nothing in the app could clear
it. A remembered package that no longer exists is now forgotten; one that was
renamed or moved is followed to its new home. A package that is still there but
cannot be reopened still fails honestly rather than being skipped.

**A failed breakdown row is logged.** A row that failed to render used to leave
no trace anywhere, so a failure could not be diagnosed after the fact. It is
logged now.
