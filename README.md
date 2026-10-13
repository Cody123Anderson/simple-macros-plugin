# Simple Macros

Track calories and macros by talking to your AI assistant. Simple Macros is a free calorie and macro tracker for iPhone, Android, and connected AI assistants.

This plugin connects to the existing Simple Macros hosted MCP server. No local server, API key, or command-line installation is required.

## What you can do

- Log meals and weigh-ins, and see them in the Simple Macros app.
- Check remaining calories and protein against your saved goals.
- Read your food log, goals, and tracking history.
- Save favorite meals and log them again.
- Find restaurant menus and calculate macros for custom orders.
- Generate restaurant meal ideas for a calorie target and protein goal.

Food data comes from USDA FoodData Central, packaged-product nutrition labels, community contributions, and published restaurant nutrition. Estimated values are labeled in tool results. Restaurant coverage varies by country and chain. The connector does not place food orders or provide medical treatment.

## Connect

1. Install the plugin from the marketplace when it becomes available. While the listing is under review, you can add the MCP server manually using the URL below.
2. Sign in to your Simple Macros account when the assistant opens the authorization page. Create an account and complete setup if needed.
3. Choose **Full access** to read and write your tracking data, or **Read-only** to view it without changes. Approve the connection.
4. Ask a question or describe a meal.

**MCP server:** `https://mcp.simplemacros.com/mcp`

The server uses Streamable HTTP and OAuth 2.1 with dynamic client registration and PKCE. Each user authorizes their own account. The plugin contains no credentials and does not change the server's access controls. You can revoke a connection in Simple Macros Settings → AI Assistants.

For a manual Cursor connection, add the contents of [mcp.json](mcp.json) to your MCP settings. Follow the current [Cursor MCP setup instructions](https://cursor.com/docs/context/mcp). Setup for other assistants is on the [Simple Macros connect page](https://simplemacros.com/connect).

## Try asking

- "How many calories and how much protein do I have left today?"
- "Log two eggs, sourdough bread, and a banana for breakfast."
- "What can I get at Chick-fil-A for around 800 calories and at least 50 grams of protein?"
- "Calculate the macros for my Chipotle bowl with extra chicken."
- "Log my favorite breakfast."
- "I weighed in at 175 pounds today. Log it."

## Documentation and support

- [Tool reference](https://simplemacros.com/docs/mcp)
- [Website](https://simplemacros.com)
- [Privacy policy](https://simplemacros.com/privacy-policy)
- [Terms of service](https://simplemacros.com/terms-of-service)
- Support: [support@simplemacros.com](mailto:support@simplemacros.com)

## Repository contents

- `.cursor-plugin/plugin.json`: marketplace metadata.
- `mcp.json`: the hosted MCP connection.
- `assets/logo.png`: the Simple Macros logo.

This repository distributes plugin configuration and documentation. The app and hosted service are maintained separately.
