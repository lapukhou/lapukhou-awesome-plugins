# lapukhou-awesome-plugins

Claude Code plugin marketplace by Ihar Lapukhou — a curated collection of awesome plugins. Plugins live in their own GitHub repositories; this repo only hosts the marketplace manifest (`.claude-plugin/marketplace.json`).

## Installation

Add the marketplace:

```
/plugin marketplace add lapukhou/lapukhou-awesome-plugins
```

Then install a plugin:

```
/plugin install swiftui-expert@lapukhou-awesome-plugins
```

## Plugins

| Plugin | Repository | Description |
| --- | --- | --- |
| `swiftui-expert` | [AvdLee/SwiftUI-Agent-Skill](https://github.com/AvdLee/SwiftUI-Agent-Skill) | Expert SwiftUI guidance for state management, view composition, performance, and iOS 26+ Liquid Glass adoption. |

## Adding a plugin

Each entry in `.claude-plugin/marketplace.json` points to an external repo:

```json
{
    "name": "plugin-name",
    "source": {
        "source": "github",
        "repo": "owner/repo"
    },
    "description": "What the plugin does."
}
```

If the plugin is not at the repo root, add a `"path"` field inside `source` pointing to the plugin subdirectory.
