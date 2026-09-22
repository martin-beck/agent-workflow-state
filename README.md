# Agent Workflow State

This repository is the Git-backed coordination state for
`martin-beck/agent-workflow`, the umbrella entry point for the Agent Workflow
family. It vendors an immutable Agent Workflow Coordinator release and stores
task records, plans, generated views, and concise public evidence for
program-level and cross-child coordination work.

Use `tools/handoffctl` from this state repository or the configured product
checkout. Never edit generated views directly and never patch files under the
vendored coordinator tree. Product, Git, review, and publication mutations
must run through `handoffctl run` for the claimed task.

The umbrella product repository is separate by design. This repository
coordinates changes to it; it is not the product source tree. Child ARs live
in each child's own state repository.
