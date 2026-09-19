# AirPrompter for Cursor

Create, run, and improve AirPrompter workflows from Cursor.

This repository is a Cursor plugin marketplace in the official plugin
format: `.cursor-plugin/marketplace.json` at the root and the plugin at
`plugins/airprompter/`.

## Install

Install AirPrompter from the Cursor Marketplace. Cursor registers the
bundled MCP server and prompts for AirPrompter account authorization.
Plugin install is separate from that authorization step; reconnect from
Customize → MCP, then start a new chat.

## What is packaged

- Plugin metadata, the AirPrompter Skill, and `mcp.json` naming the hosted
  AirPrompter MCP server.
- No credentials, client ids, scopes, or customer identifiers.

See `INSTALL.md` for maintainer validation and submission notes.
