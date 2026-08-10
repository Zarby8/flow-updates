# FLOW 1.0.729

- Fixes the preview-player crash caused when AVFoundation saw one video item attached to two player instances.
- Keeps each preview item with one player from readiness through playback across IQ Library, NHL search, NHL database, and Organizer previews.
- Preserves the prior visible frame while a replacement preview loads, with normal audio and playback controls after the swap.

This update changes no project schema or media format. Existing databases and packages remain compatible, and signed build 728 is retained for rollback.
