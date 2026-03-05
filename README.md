# claude-plugins

A marketplace of Claude Code plugins by guyvinograd.

## Installation

First, register this marketplace in Claude Code (one-time setup):

Add the following to `~/.claude/plugins/known_marketplaces.json`:

```json
"guyvinograd": {
  "source": {
    "source": "github",
    "repo": "guyvinograd/claude-plugins"
  }
}
```

Then install any plugin with:

```
/plugin install <plugin-name>@guyvinograd
```

## Plugins

| Plugin | Description |
|--------|-------------|
| [say-plugin](./plugins/say-plugin) | Speak text aloud via Windows TTS |

## Notes

- Plugins use `"strict": false`, meaning Claude uses judgment about when to invoke a skill rather than requiring an exact trigger phrase.

