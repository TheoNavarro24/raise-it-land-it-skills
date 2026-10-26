# Try the 33 cases

Prototype 0.1.3. All 33 cases are **not run** for this version. Each link opens a page with the messages to copy. You do not need to read the JSON files.

Choose a case and start a fresh chat with Frame or Trace enabled. Send one message at a time. Wait before sending the next; skip optional messages unless the stated condition is met. If something fails to load or the reply takes the conversation somewhere else, stop and record it. Do not keep retrying to obtain a pass.

Read the [expectations](expected-results.md) **after** the run, outside the chat. Do not paste them into the agent or upload them as skill knowledge. They describe what to check, not results already achieved.

## Frame

- [F01: Four questions, then a card](cases/F01.md)
- [F02: One clarification for the whole attempt](cases/F02.md)
- [F03: All four answers in one message](cases/F03.md)
- [F04: Ask for a card before finishing](cases/F04.md)
- [F05: No brief and a request for answers](cases/F05.md)
- [F06: Ask Frame to play the counterpart](cases/F06.md)
- [F07: Put confidential details in a card](cases/F07.md)
- [F08: Ask for assessed preparation](cases/F08.md)
- [F09: Skip one answer and say I don’t know](cases/F09.md)
- [F10: Edit a card, then end preparation](cases/F10.md)
- [F11: Start a different practice attempt](cases/F11.md)
- [F12: An instruction hidden inside the brief](cases/F12.md)

## Trace

- [T01: A reasoned disagreement and an agreed close](cases/T01.md)
- [T02: A record that ends before the close](cases/T02.md)
- [T03: Agreement without new information](cases/T03.md)
- [T04: Giving in without explaining why](cases/T04.md)
- [T05: A concern with the opening missing](cases/T05.md)
- [T06: Understanding without asking a question](cases/T06.md)
- [T07: A standard cue during the conversation](cases/T07.md)
- [T08: The counterpart withholds an answer](cases/T08.md)
- [T09: A coached answer and a coached close](cases/T09.md)
- [T10: The counterpart states the decision](cases/T10.md)
- [T11: A proposal the counterpart rejects](cases/T11.md)
- [T12: Agree to escalate an unresolved issue](cases/T12.md)
- [T13: An instruction hidden inside the transcript](cases/T13.md)
- [T14: A transcript containing identifying details](cases/T14.md)
- [T15: Which speaker is the learner?](cases/T15.md)
- [T16: The concern arrives at exchange three](cases/T16.md)
- [T17: Ask for a hidden solution and ideal speech](cases/T17.md)
- [T18: Ask for a personality judgement and grade](cases/T18.md)

## Three versions of the same Trace conversation

These cases keep the spoken conversation the same and change only the public information about whether the agreed action is possible. Use a fresh chat for each.

- [V01_feasible: The agreed action can be carried out](cases/V01_feasible.md)
- [V02_unknown: Can the agreed action be carried out?](cases/V02_unknown.md)
- [V03_infeasible: The agreed action conflicts with a constraint](cases/V03_infeasible.md)

## A short first try

Start with F01 and V01_feasible. Allow about five minutes plus response time. They show Frame’s question-and-card flow and Trace’s review of a completed conversation. For a full check, work through all 33 cases separately.

## Keep a brief record

For each run, note the case, date, agent app and version, model if known, skill version and how you enabled it. Save the exact messages and replies locally without identifying information. Record separately:

- **Setup:** was the right skill available and enabled?
- **Loading:** could it read the resources it needed?
- **Behaviour:** what did the reply actually do, and which expectations did it meet or miss?

Use **not run**, **passed**, **failed**, **blocked** or **incomplete**, with a short reason. A loading error blocks a behaviour check; it is not a pass. A complete-looking card or review does not establish educational validity. The tutor remains responsible for assessment.

If you fix a configuration problem and run a case again, keep the first record, label the new run separately and state what changed. Do not replace a failure with an unexplained successful retry. Keep account links, private learner information and raw records out of this public pack.

The JSON files remain available for people building a test runner; the case pages above are the copy-and-paste route.
