# Install and try the prototypes

These instructions are for prototype 0.1.2. Installation steps are based on official product documentation checked on 26 October 2026; they have not been verified in your account. Menus and access can vary. Neither route requires you to paste the skills' operating instructions into a chat.

## Option A — Claude custom-skill upload

1. Download `frame-agent-skill-0.1.2.zip` and `trace-agent-skill-0.1.2.zip` from [release 0.1.2](https://github.com/TheoNavarro24/raise-it-land-it-skills/releases/tag/v0.1.2). Use the individual skill ZIPs, not the complete prototype pack or GitHub's whole-repository source ZIP.
2. In Claude, open **Customize → Skills → + → Create skill → Upload a skill**. Upload each ZIP separately and enable it.
3. If Skills is unavailable, check the account's **Code execution and file creation / Create and edit files** capability. An organisation may control access. Follow the [official Claude skill instructions](https://support.claude.com/en/articles/12512180-use-skills-in-claude) for your account.
4. Start a fresh conversation. Ask to use **Frame** for the [Frame example](examples/frame-cycle1.md), or **Trace** for the [Trace example](examples/trace-demo.md). Confirm the host selected the intended skill before judging its behaviour.

Each ZIP contains one folder, `frame/` or `trace/`, with `SKILL.md` and its supporting files. The host may provide code execution for skill/file access; these skills contain no executable scripts.

## Option B — local Codex skill installation

In a local Codex session with the built-in skill installer, request:

```text
$skill-installer Install the frame and trace skills from https://github.com/TheoNavarro24/raise-it-land-it-skills, using skills/frame and skills/trace. Keep both complete folders and their supporting files.
```

Alternatively, download and extract the individual ZIPs. Place the resulting `frame` and `trace` folders in the documented user skills location, `~/.agents/skills/`, without overwriting an existing installation accidentally. The final paths should include `~/.agents/skills/frame/SKILL.md` and `~/.agents/skills/trace/SKILL.md`. Restart Codex if the skills do not appear.

Start a fresh conversation and select the intended skill, or explicitly invoke `$frame` / `$trace` before sending its example input. See the [official OpenAI skill documentation](https://learn.chatgpt.com/docs/build-skills) for discovery and installation details.

## Other hosts, including ChatGPT

Use another host only if it supports custom Agent Skills and can read the complete skill folder. Follow that host's installation flow. A standalone skill ZIP is not a ChatGPT plugin ZIP, and a GitHub URL is not an installed assistant. This release does not claim a verified ChatGPT web installation route or recipient-account access.

## First-use check

Confirm which skill is active and the release being tested. Frame has its main workflow inline; Trace requires its four packaged resources and must stop if they cannot be read. If skill selection or resource access fails, record **SETUP_BLOCKED** rather than proceeding as though the skill loaded. Then follow [the test guide](tests/README.md).

Use a separate fresh conversation for each Frame attempt or Trace run. Do not load test expectations as runtime knowledge. After updating an existing installation, confirm the host uses 0.1.2 rather than a cached or duplicate 0.1.1 skill.
