# starside plugins

The Claude Code plugin marketplace for [starside.io](https://starside.io).

## Install

```
/plugin marketplace add starside-io/claude-plugins
```

Then install what you want:

```
/plugin install neurowire@starside
/plugin install ghostwriter@starside
/plugin install fellowship@starside
```

## What is here

| Plugin | What it does | Source |
|--------|--------------|--------|
| `neurowire` | Clean feeds from any blog, site, RSS, or Atom source. Bundles the `@neurowire/mcp` server (feeds, meshes, journals with cursors, tap verification) with skills for following feeds and authoring taps. | [starside-io/neurowire](https://github.com/starside-io/neurowire) |
| `ghostwriter` | Makes generated text read as human-written, with none of the punctuation, rhythm, or vocabulary tells. | [starside-io/ghostwriter](https://github.com/starside-io/ghostwriter) |
| `fellowship` | A local-first record of the people in your life: facts, likes and allergies, shared occasions and closeness. Bundles the Fellowship MCP server (42 tools) with skills for setup, chat recaps, sketches and personality radars. Every draft waits for your yes. | [starside-io/fellowship](https://github.com/starside-io/fellowship) |

Each plugin lives in its own repository. This one holds only the catalog, so a
plugin ships on its own schedule and installs resolve to its latest commit.

## Adding a plugin

Add an entry to `.claude-plugin/marketplace.json`, then check it before pushing:

```
claude plugin validate .
```

Names must be unique and kebab-case, and every source must resolve.
