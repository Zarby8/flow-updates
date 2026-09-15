# FLOW 1.0.1464

**Cockpit panels always fit the window.** The code rail, the stage, and the BOB
panel now share the window through a real width budget. If your saved panel
widths are wider than the display, the panels give width back to the stage
instead of pushing BOB off the screen — that is why BOB's read could be cut off
and the panel could not be brought back in full-screen mode. Your saved layout
is never rewritten; the panels return to their sizes as soon as the window can
hold them.

**Timeline toolbar wraps.** The five brand groups (BUILD · REVIEW · NOTES ·
INTEL · DELIVER) stay on one evenly spread row when they fit and wrap onto
another line when they do not, instead of running off the right edge.

**Timeline row names stay readable.** A clip that starts before the visible
window is clipped to its own lane, so it can no longer paint over the row name.

**Full-screen identity stays centred.** The project title above the stage is
centred on the stage you actually see, including when the panels yield.
