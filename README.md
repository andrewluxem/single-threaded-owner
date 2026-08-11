# single-threaded-owner

Defines one accountable owner, authority boundary, measures, interfaces, and escalation path.

It produces:

- **Single Threaded Owner Charter:** a working artifact built from supplied facts, labeled inference, and visible missing fields.

It executes the [Single Threaded Owner playbook](https://www.andrewluxem.com/playbooks/single-threaded-owner). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/single-threaded-owner.git
cp -r single-threaded-owner/skills/single-threaded-owner ~/.claude/skills/
```

For Codex, copy the same complete folder to the Codex skills directory:

```bash
cp -r single-threaded-owner/skills/single-threaded-owner ~/.codex/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/single-threaded-owner
/plugin install single-threaded-owner@single-threaded-owner
```

For clients that install from an archive, use the versioned [single-threaded-owner v1.0.0 ZIP](https://www.andrewluxem.com/downloads/single-threaded-owner-v1.0.0.zip).

## Invoke it

```text
Write the single threaded owner charter for this program
Use the single-threaded-owner skill.
```

Naming the skill is always valid: `use the single-threaded-owner skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/single-threaded-owner/
  assets/single-threaded-owner-charter-template.md
  LICENSE.md
  meta.yaml
  references/owner-charter-standard.md
  SKILL.md
README.md
LICENSE
```

The complete canonical package is copied under `skills/single-threaded-owner/`, including every asset, reference, test prompt, source note, changelog entry, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, `.claude-plugin/plugin.json`, and `.claude-plugin/marketplace.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/single-threaded-owner/LICENSE.md](skills/single-threaded-owner/LICENSE.md).
