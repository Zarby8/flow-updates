# FLOW 1.0.1468

**Each Mac files into its own NAS space.** FLOW now resolves its owner — Shane on
Shane's Mac, Chris on Chris's — and uses that to choose the client folder it files
breakdowns into, the taxonomy export it reads, and the week-prep folders it writes.
Before this, those paths were fixed to Chris's tree, which on Shane's Mac would have
sent his breakdowns into Chris's clients. FLOW now refuses outright to file into the
other coach's private root.

**Settings → Diagnostics shows the wiring.** A new MACHINE WIRING block lists the
coach, the private NAS root, the client roster it resolved, whether that roster is
mounted, the fallback folders and the taxonomy export — and COPY DIAGNOSTICS leads
with the same line. So "is this Mac wired correctly?" is answerable on the machine
itself.

**Also in this build:** the roster lookup prefers a folder that actually contains
clients (Shane's machine has an empty older-season folder next to a populated one),
and an override exists for operators: `FORCEIQ_FLOW_OWNER`,
`FORCEIQ_FLOW_CLIENT_ROSTER_ROOT`, `FORCEIQ_FLOW_NAS_PRIVATE_ROOT`.
