# Frame and Trace — educational prototypes

**MDOE407 midterm project · Raise It, Land It · Prototype release 0.1.2**

Frame and Trace demonstrate two proposed uses of AI in a course about raising a concern, investigating it and reaching a workable decision. These are experimental Agent Skills for demonstration and testing. They are not validated teaching or assessment products, and they do not grade learners.

| Skill | Who uses it and when? | What should it produce? |
|---|---|---|
| **Frame** | A learner, before cycle 1 formative practice | A four-field preparation card containing the learner's own words. It asks questions; it does not supply arguments or coach an opening. |
| **Trace** | A tutor, after a role-play has ended | An advisory review with exact transcript quotations, marker evidence, uncertainty and checks for the tutor. The tutor decides assessment. |

## Start here

1. **Install once:** download the individual [Frame and Trace skill ZIPs](https://github.com/TheoNavarro24/raise-it-land-it-skills/releases/tag/v0.1.2). Follow [INSTALL.md](INSTALL.md) for the documented Claude or local Codex route. You need an account/app that supports custom skills.
2. **Try Frame:** activate Frame in a fresh conversation and follow [the staged Frame example](examples/frame-cycle1.md). Send one learner reply at a time, waiting for its question. The fourth reply should produce the card automatically.
3. **Try Trace:** activate Trace in another fresh conversation and send [the complete fictional demo transcript](examples/trace-demo.md). Inspect the review and its five-part decision check.
4. **Check the result:** use [the test guide](tests/README.md) and its separate expectations. Record the result in the supplied log template. Loading errors are blocked tests, not evidence that the behaviour passed.

For a single download containing the documentation, skills and all test cases, choose `Frame-Trace-Prototype-Pack-0.1.2.zip` from the same release. Import only the individual skill ZIPs into a host.

Allow about five minutes **after installation**, plus model generation time. The example text is fictional input for a demonstration, not an assessed learner's answer key. You can type your own permitted input instead.

**The installation loads the operating instructions.** You do not need to paste `SKILL.md` into every conversation. The examples contain the brief, learner replies or transcript you send during a test.

## What the links and downloads do

The GitHub links let you inspect and download the skills. They do not launch a hosted chatbot or give access to private ChatGPT plugins. Install each complete skill folder in a compatible host before using it. The ZIPs contain instructions, references and templates; there is no custom server, executable script or API key in this repository.

The file format is portable across compatible agents. Actual installation, file access, skill selection and model behaviour depend on the host. The documented installation routes have not been tested in a recipient's account. ChatGPT web plugin installation is not established by publishing these standalone folders.

## What has actually been verified?

Earlier **0.1.1 private ChatGPT plugin** attempts included a complete Frame workflow and a complete Trace review where feasibility was unknown. Other attempts failed to load. Those results do not establish that this public release works in another host.

**0.1.2 adds clearer prototype instructions, installation guidance and a revised test pack. Its behavioural cases start as NOT_RUN.** File validation and independent review are different from a live user test. See [VALIDATION.md](VALIDATION.md) for evidence and limits.

## Scope for this prototype

- Use fictional demonstration material. Frame supports cycle 1 formative preparation; assessed/cycle 2 preparation and live calls are outside its scope.
- Trace can support tutor review after either practice or an assessed run has ended. It never assists the assessed performance or produces an official grade.
- A reasoned change, refinement or retention after new information may support **Move**. A concession is not required.
- **Land it** requires evidence of a decision, owner, observable review condition, agreement and feasibility. An ownership promise alone does not establish feasibility.
- The facilitator controls timing and card handling. The tutor checks evidence and decides assessment. These instructions do not technically enforce those responsibilities.

## Files

```text
skills/frame/       Installable Frame skill: SKILL.md, scope reference, card template
skills/trace/       Installable Trace skill: SKILL.md, rubric, protocol, review template
examples/           Fictional inputs for the short demonstration
tests/              Staged regression inputs, separate expectations and result log
INSTALL.md          Installation and first-use instructions
VALIDATION.md       Evidence, version distinctions and known limitations
CHANGELOG.md        Changes to the prototype
```

Keep `examples/` and `tests/` outside the installed skill folders. In a blind test, the agent receives the skill and case input; the human reviewer keeps expected results separate. Report a problem with the release, host/model, case ID, observed response and expected check. Do not post real learner or workplace records in a public issue.
