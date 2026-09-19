# Setup Diagnostics

Use this reference when AirPrompter tools are missing, or when the user asks
to diagnose, repair, reconnect, or reinstall AirPrompter in Cursor.

## Readiness Layers

Treat the Skill, MCP server definition, OAuth session, and live tool
inventory as separate states. A Skill-only install cannot call AirPrompter.

1. Open Customize and confirm the AirPrompter plugin is installed.
2. Confirm the bundled MCP server `airprompter` points at
   `https://mcp.airprompter.com/mcp`.
3. Run `diagnose_connection` through the host before executing a saved
   workflow. Tool discovery alone does not prove authentication.
4. Start a new Cursor chat after reconnecting. The tool inventory for a
   running chat is fixed when that chat starts.

## Customer Installation

Install AirPrompter from the Cursor Marketplace (Customize → Plugins), then
approve AirPrompter account authorization when Cursor prompts. Customers
must not paste tokens, edit `mcp.json`, or register a second MCP server.

## Reconnect

If tools return Unauthorized after a completed login, open Customize → MCP,
reconnect AirPrompter, and start a new chat. Package reinstall and MCP
authentication are independent.

## Maintainer Local Validation

Copy the generated plugin directory to `~/.cursor/plugins/local/<pluginName>`
and reload the Cursor window. Cursor skips symlinks that point outside that
folder. Local plugin imports may be disabled on Enterprise.
