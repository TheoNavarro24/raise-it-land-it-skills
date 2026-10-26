# Install Frame and Trace

Install the skills once, then use them in ordinary conversations. You won't need to paste their instruction files into each chat.

The steps below follow the products' published instructions, checked on 26 October 2026. I haven't yet tested installation in another person's account.

## Using Claude

1. Open [the downloads](https://github.com/TheoNavarro24/raise-it-land-it-skills/releases/tag/v0.1.3).
2. Download **frame-agent-skill-0.1.3.zip** and **trace-agent-skill-0.1.3.zip**. Leave them zipped.
3. In Claude, go to **Customize → Skills**. Click **+**, then **Create skill → Upload a skill**.
4. Upload each ZIP separately and turn both skills on.
5. Start a new chat. Ask Claude to use Frame or Trace, then follow [the Frame example](examples/frame-cycle1.md) or [the Trace example](examples/trace-demo.md).

If you don't see Skills, check whether **Code execution and file creation** (sometimes called **Create and edit files**) is enabled in your settings. A work or university account may have different permissions. [Claude's instructions](https://support.claude.com/en/articles/12512180-use-skills-in-claude) explain those settings.

## Using local Codex

Ask the built-in skill installer:

```text
$skill-installer Install frame and trace from https://github.com/TheoNavarro24/raise-it-land-it-skills using the skills/frame and skills/trace folders.
```

Then start a new conversation and select Frame or Trace. You can also invoke `$frame` or `$trace` explicitly.

For a manual installation, extract the individual ZIPs into `~/.agents/skills/`. You should end up with `frame/SKILL.md` and `trace/SKILL.md` inside that folder, alongside their supporting files. Check for an existing copy before replacing it. Restart Codex if the skills don't appear. See [OpenAI's installation guidance](https://learn.chatgpt.com/docs/build-skills).

## Which download do I need?

- **Frame ZIP:** the Frame skill, ready to import.
- **Trace ZIP:** the Trace skill, ready to import.
- **Frame-Trace-Prototype-Pack ZIP:** both skill folders, the examples and all 33 tests. Extract this to browse the project; don't upload the whole pack as one skill.

Other apps may support the same skill folders. Follow their installation instructions and keep each skill's files together. A skill ZIP is different from a ChatGPT plugin ZIP; these downloads don't give access to the private ChatGPT plugins.

If the app can't find a skill or read its files, stop there and note the problem. Otherwise, [try the examples](README.md#try-them).
