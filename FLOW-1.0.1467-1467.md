# FLOW 1.0.1467

**The breakdown progress bar now tells the truth.** It used to climb to 100% and
then drop back to 0% part-way through, because each internal step reported its own
percentage. It is now one bar for the whole job: it names the row it is on
(`ROW 2 OF 5`) and the step it is running (rendering clips, assembling the row,
embedding chapters), and it only ever moves forward.

**NAS delivery is more reliable and no longer silent about failure.** A copy that
is interrupted (for example by a dropped network session) is retried once
automatically instead of failing, and if it still cannot finish it says so with
the reason, keeps your local movie, and clears its own temporary files so nothing
is left behind in the game folder. If the movie is already on the NAS, FLOW now
says so and tidies any leftovers from an earlier attempt.
