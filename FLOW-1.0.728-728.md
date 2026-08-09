# FLOW 1.0.728

- Declares FLOW's two app-owned NHL transfer types in the signed application bundle, eliminating Launch Services' runtime type-declaration warning.
- Hardens code-button grid measurement and placement against transient zero, narrow, negative, and nonfinite layout proposals so the cockpit never emits invalid button dimensions.
- Preserves build 727's canonical client code windows, full video controls, manual `_All-Shifts.mov` export, timeline/package workflow, GHOST-backed pre-scout context, and Automark review path.

This update changes no project schema or media format. The existing database, packages, and build-727 rollback artifact remain compatible.
