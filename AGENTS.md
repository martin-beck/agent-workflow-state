# Coordination instructions

Read `docs/agent-workflow-coordinator.md`, the complete generated snapshot,
the selected task, and its plan before work. Claim exactly one dependency-ready
task. Route every product, Git, review, and publication mutation through
`tools/handoffctl run`.

This state repository tracks umbrella-level ARs only (manifest, compatibility,
pipeline, dogfooding, and cross-child contracts). Child implementation ARs
belong to the respective child state repositories. Keep task evidence concise
and public-safe. Preserve signed, DCO-certified commits, immutable vendor
pins, and exact-head review evidence. Do not edit generated views or vendored
coordinator files.
