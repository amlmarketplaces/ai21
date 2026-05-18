# amlmarketplaces/ai21

Claude Code marketplace federating all `@amlplugins/ai21-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-ai21": {
      "source": { "source": "github", "repo": "amlmarketplaces/ai21" }
    }
  },
  "enabledPlugins": {
      "ai21-chat@aml-ai21": true,
      "ai21-conversational-rag@aml-ai21": true,
      "ai21-library@aml-ai21": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/ai21`, cached under `~/.claude/plugins/cache/aml-ai21/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (3 total)

- `ai21-chat` — [@amlplugins/ai21-chat](https://github.com/amlplugins/ai21-chat)
- `ai21-conversational-rag` — [@amlplugins/ai21-conversational-rag](https://github.com/amlplugins/ai21-conversational-rag)
- `ai21-library` — [@amlplugins/ai21-library](https://github.com/amlplugins/ai21-library)

## Related

- npm packages: `@amlplugins/ai21-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
