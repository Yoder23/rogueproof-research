# Rogueproof

**An AI agent should stop when its reason for acting is no longer valid—and find a justified way to finish the job.**

Rogueproof is a research project on agents that respond to revoked authority, corrected evidence, and changing task constraints. We aim to measure whether explicit justification tracking improves action selection and recovery while preserving useful task completion.

**Current status: research plan published; prepared source bundle import pending.** This checkout contains the execution plan and project backlog. The accepted implementation, deterministic demo, historical traces, and retained test reports will be imported from the separately prepared source bundle. They are not yet available in this checkout. No learned-avoidance result or universal safety guarantee is claimed.

## Start here

Read [the breakthrough execution plan](docs/BREAKTHROUGH_EXECUTION_PLAN.md) for the experiment design, evidence gates, proposed success criteria, resource limits, and first implementation work. [Source import status](docs/SOURCE_IMPORT.md) identifies the exact prepared bundle and verification requirements.

## The behavior we want to demonstrate

Imagine an agent preparing a report for delivery. Permission is withdrawn before it sends the report, or new evidence invalidates part of its reasoning. The agent should recognize the change, withhold the stale action, and choose a permitted alternative using current evidence and authority.

We will test both removal and restoration of valid support. An agent that refuses everything cannot satisfy the useful-completion criteria. A forged instruction inside untrusted content must not be treated as an authorized correction.

The human analogy motivates a testable behavior. It does not establish that an AI has a conscience or human moral understanding. In the initial experiments, wrongful means a violation of a declared task policy, authority rule, or evidence requirement. Defining those requirements remains a human responsibility.

## What would count as progress

| Stage | Evidence |
| --- | --- |
| Reliable boundary | Invalid actions produce no prohibited effects within the declared simulator; valid actions still succeed |
| Better action selection | Fewer invalid proposals before external gate intervention, with useful completion preserved at matched budgets |
| Learned transfer | A trained policy improves on unseen task and constraint families against matched training controls |

These are separate research claims. The proposed measurements, task splits, controls, uncertainty estimates, and stop conditions are in the execution plan. Proposed thresholds are not results.

## First milestone

Reproduce and resolve the retained machine/custody discrepancy using an independent world-state observer. Then build strong controls and a small paired pilot before freezing a held-out confirmation study.

Runtime rules, behavioral contracts, and interruption have direct precedents. Our candidate contribution must be established through a specific comparative result and reproducible evidence. The plan links primary sources and states exactly what was reviewed.

## Contributing

Start with a backlog item in the execution plan and its definition of done. Preserve original research records, separate proposed work from observed results, and include failures and incomplete episodes in the evaluation record. Model campaigns need a declared protocol and total cost ceiling. This planning checkout has no model runner or automated test workflow yet.

## License status

A project license has not been selected. The prepared bundle's license-status documentation will be included with the source import. Public visibility does not itself specify reuse permissions.
