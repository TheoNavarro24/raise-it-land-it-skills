# Validation and limits

Version 0.1.1. Status recorded 26 October 2026.

## Candidate checks

The `skills/frame` and `skills/trace` contents were copied byte-for-byte from the actual version 0.1.1 skill packages, retaining their YAML name/description, instructions, references and assets. No platform manifest, account metadata, conversation log, generated response, binary package, native GPT adaptation or expected output is included in those skill folders. Skill source names its version as a string; no new metadata schema was invented.

Example Frame inputs are fictional. The three Trace inputs are copied exactly from the existing feasibility cases; expected dispositions are separate under `tests/`. Packaging checks verify source equality, required local links/resources and input fidelity. These checks establish file integrity, not runtime behaviour.

## Existing runtime evidence

Creator-account ChatGPT tests of the private installed version 0.1.1 produced a completed Frame workflow in Work and a completed Trace review with feasibility unknown. Those are platform-specific observations, not tests of this public repository installed in another agent. Other attempts, including Trace’s contradicted-feasibility case in Thinking and Instant, returned loading errors. A reduced ordinary-chat Frame demonstration completed four questions and an automatic literal card; reduced prompts are separate adaptations and are not included as skills here. Reduced Trace attempts returned loading errors. Full portable Trace was not executed.

The candidate repository has not been installed or tested across providers or on a recipient’s account. Not all example cases or optional boundary checks have passed live tests. No numerical reliability/fairness claim follows from a completed review or these files.

## Suggested recipient check

After installation, confirm the chosen skill activates and can read required resources. Use the fictional examples and inspect the separate expected-behaviour checks. Record the agent/version, observed output and limits without treating skill loading or template completion as educational validation. Tutors verify exact quotations, context and interpretation before use; official assessment remains human.
