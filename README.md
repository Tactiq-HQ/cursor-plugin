# Tactiq for Cursor

Bring your meetings into Cursor. This plugin connects Cursor's agent to the [Tactiq](https://tactiq.io) MCP server, so it can search your meetings and read their summaries, action items, transcripts and AI artifacts while you work.

## What you can ask

- "What did we decide about the export API in yesterday's planning meeting?"
- "Pull the action items from my last call with Acme and add them as TODOs in this repo."
- "Find where the customer described the login bug and quote it."

## Install

Install **Tactiq** from the Cursor Marketplace. The first time the agent uses a Tactiq tool, Cursor opens your browser so you can sign in to Tactiq and approve access.

To add the server by hand instead, put this in `.cursor/mcp.json` for one project or `~/.cursor/mcp.json` for all of them:

```json
{
  "mcpServers": {
    "tactiq": {
      "url": "https://mcp.tactiq.io"
    }
  }
}
```

## What the agent can do

- Search your meetings, or list the most recent ones
- Read a meeting's summary and action items
- Read AI artifacts generated for a meeting
- Read a full transcript, or just the excerpts that answer a question
- Browse your team's spaces

Results include a link back to the meeting in Tactiq, so you can check the source.

Some tools depend on your Tactiq plan. When one isn't available to you, Tactiq tells you what unlocks it.

## Learn more

- [Connecting the Tactiq MCP server](https://tactiq.io/help/mcp)
- Questions or problems: [hello@tactiq.io](mailto:hello@tactiq.io)

## License

[MIT](LICENSE)
