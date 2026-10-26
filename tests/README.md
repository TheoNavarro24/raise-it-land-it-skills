# Prototype test pack 0.1.2

There are 33 staged cases: original IDs F01–F12 and T01–T18 plus explicit feasibility variants V01_feasible, V02_unknown and V03_infeasible. Every version 0.1.2 case is **NOT_RUN**. Prior ChatGPT observations do not count as these cases passing, and this pack makes no cross-provider reliability claim.

## Five-minute check

1. In a compatible agent, install/select Frame and follow [the Frame example](../examples/frame-cycle1.md) in a fresh conversation. Send each reply only when its question appears; wait for the card after reply four.
2. Install/select Trace in a separate fresh conversation and send only the input block from [the Trace example](../examples/trace-demo.md). Wait for the review or resource/loading limitation.
3. Outside the agent conversation, compare with the common criteria and relevant cases in expected-results.json. Record host/version/model and what occurred. Five minutes is a route estimate, not a generation-time guarantee.

## Full regression

Keep inputs.json and expected-results.json separate. The person/agent executing inputs must not see acceptance criteria in its runtime context. A reviewer may read them outside that context. Do not install tests/ or examples/ as skill knowledge.

For each case, start a fresh conversation, select the named skill using the host’s native mechanism and record setup. Send the first stage only. Wait for the actual response, then send the next stage only if its send_when condition is met. Optional clarification stages are conditional; never send them when the agent did not ask. Do not paste all staged messages at once, invent responses, reveal criteria or force unexpected questions into the planned sequence. On an unreachable continuation, stop and record where it diverged.

Record setup/loading failures separately from observable behaviour. Do not retry a failed case repeatedly to obtain a pass. Preserve the first result; if an independently justified configuration repair warrants rerunning, use a new run ID, state the change and retain the earlier failure. An unavailable skill/resource is not a behavioural pass. A generated template is not educational validation.

After one complete case, a reviewer checks exact quotes, sources, marker components and boundaries against the criteria. Use PASS only if all applicable criteria were inspected and met. Use FAIL for observed behavioural contradictions, BLOCKED for a setup/load limitation preventing assessment, and INCOMPLETE when interrupted/unreachable before a decision; keep NOT_RUN until an attempt occurs. Record mixed observations rather than hiding them in a single label. Human tutor assessment remains separate.

## Overall result labels

| Label | Use it when |
|---|---|
| NOT_RUN | No attempt has been made. |
| SETUP_BLOCKED | Installation, skill selection or required resource access failed. |
| LOADING_BLOCKED | A response failed to load, preventing behavioural review. |
| INCOMPLETE | The attempt ended or diverged before enough evidence was available. Record any observed failure separately. |
| PASS | A reviewer checked every applicable criterion and found supporting evidence. |
| FAIL | The observed response contradicts an applicable behavioural criterion. |

A run may contain partial observations even when its overall result is blocked or incomplete. Keep those notes and the setup/load/behaviour fields below; do not convert them into a pass.

## Run record template

Copy this template into a separate local record; do not submit it to the agent as instructions or commit personal/account information.

```text
Run ID / date / tester:
Pack version: 0.1.2
Case ID:
Overall result: NOT_RUN / SETUP_BLOCKED / LOADING_BLOCKED / INCOMPLETE / PASS / FAIL
Host and version:
Model and version (or unknown):
Skill installation/source revision:
Native skill-selection method:
Conversation/reset method:
Setup status: NOT_RUN / READY / BLOCKED
Load status: NOT_RUN / LOADED / BLOCKED / UNKNOWN
Execution status: NOT_RUN / COMPLETED / BLOCKED / INCOMPLETE
Behaviour review: NOT_REVIEWED / PASS / FAIL / PARTIAL
Stages sent and actual response locators:
Observed output (deidentified, exact record stored locally):
Criteria checked and evidence:
Unexpected question / missing resource / load error:
Limits and untested components:
Configuration changes / related earlier run ID (if any):
Reviewer and date:
```

Keep raw runs local and deidentified. No account links, identifying learner records, private counterpart content or assessed answer keys belong in this public test pack. Loading, behaviour and official assessment are different findings.
