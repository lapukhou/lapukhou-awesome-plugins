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
| `swift-concurrency` | [AvdLee/Swift-Concurrency-Agent-Skill](https://github.com/AvdLee/Swift-Concurrency-Agent-Skill) | Swift Concurrency guidance: actors, async/await, Sendable, and strict concurrency migration. |
| `xcode-build-skills` | [AvdLee/Xcode-Build-Optimization-Agent-Skill](https://github.com/AvdLee/Xcode-Build-Optimization-Agent-Skill) | Xcode build optimization and troubleshooting skills. |
| `swift-testing-expert` | [AvdLee/Swift-Testing-Agent-Skill](https://github.com/AvdLee/Swift-Testing-Agent-Skill) | Swift Testing framework guidance and migration from XCTest. |
| `core-data-expert` | [AvdLee/Core-Data-Agent-Skill](https://github.com/AvdLee/Core-Data-Agent-Skill) | Core Data best practices, migrations, and performance. |
| `mattpocock-skills` | [mattpocock/skills](https://github.com/mattpocock/skills) | Matt Pocock's engineering and productivity skills: TDD, code review, triage, domain modeling, PRDs, and more. |
| `tree-ring-memory` | [TerminallyLazy/tree-ring-memory-claude-plugin](https://github.com/TerminallyLazy/tree-ring-memory-claude-plugin) | Local-first memory lifecycle guidance for Claude Code agents using Tree Ring Memory. |

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
