# Recipe Scaler

![Recipe Scaler logo](assets/logo.png)

Search, scale, import, and shop your recipes from a Claude conversation, and run cooking timers while you cook. The plugin connects Claude to your [Recipe Scaler](https://recipe-scaler.ru) account.

## Use it

Connect Recipe Scaler from the plugin's Connectors tab and approve access on the Recipe Scaler screen. Then ask Claude to find a recipe and scale it, paste a recipe to save it, add ingredients to your shopping list, or start a timer. Recipes you change in chat show up in the Recipe Scaler web app and mobile apps.

## Contents

- `.claude-plugin/plugin.json` — plugin manifest.
- `.mcp.json` — the Recipe Scaler MCP server, `https://mcp.recipe-scaler.ru/mcp` (Streamable HTTP, OAuth).
- `skills/kitchen/SKILL.md` — instructions for using the tools.
- `assets/` — Recipe Scaler logo (PNG 512×512, SVG).

The plugin has no hooks, scripts, or local code. It runs nothing on your machine.

## Data

The plugin files do not store your recipes. Claude sends recipe, shopping-list, collection, timer, and profile requests to your Recipe Scaler account through https://mcp.recipe-scaler.ru/mcp. Import from a URL also fetches that public page so the recipe can be saved. Disconnect the connector in Claude, or delete your Recipe Scaler account, to stop access. Details are in the privacy policy at https://recipe-scaler.ru/privacy.

## Support

https://recipe-scaler.ru/about
