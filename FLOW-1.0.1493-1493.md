# FLOW 1.0.1493

**Packages open again, and the labels come back.** A package made by the provider
media intake named its client only inside its own Code Window layout — the
project row was never linked and the package carried no client record — so FLOW
refused the whole package with *"package layout is not in coach's scope."* FLOW
now reads the client from the layout, and only accepts it when it names exactly
one client on the coach's roster. A layout naming somebody outside the roster,
or two layouts that disagree, still fail closed rather than guessing.

The same defect was blanking the profile auto-labels: the strip resolves the
client from the project row, so with the row unlinked it had nothing to render.
The import now writes that link onto the project itself, so opening the package
restores the labels as well.

**One game, one project.** Importing a game that FLOW already has used to stand up
a **second** project for it, which is how a session can look like the clips are
gone — the empty twin opens and the real one is right there beside it. An import
now finds the existing project for the same game and attaches to it. Attaching
never touches that project's media or clips; it only decides which project the
package belongs to. If FLOW finds more than one project for the same game it
refuses rather than adding another, and says so.

**Title slides render for teams the artwork catalog does not carry.** The client's
own team crest was required to verify, while the opponent's was allowed to fall
back to a typographic monogram — so a team the catalog simply has no crest for
failed the whole slide. Both sides now fall back the same way. A crest that is
merely *unavailable*, or that matches more than one team, still fails honestly
rather than being invented.
