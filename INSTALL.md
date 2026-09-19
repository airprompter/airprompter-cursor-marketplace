# AirPrompter Cursor Plugin Marketplace Package

This generated marketplace follows Cursor's official plugin format:
`.cursor-plugin/marketplace.json` at the repository root and one plugin
under `plugins/`. Submit the production output as a public Git repository
at https://cursor.com/marketplace/publish.

## Customer installation

After AirPrompter is listed, customers install it once from the Cursor
Marketplace. Cursor registers the bundled MCP connection and requests
AirPrompter account authorization during installation or first tool use.
Customers must not edit `mcp.json`, paste tokens, or register the MCP
server separately.

This production output is submission and prepublication validation
input. Use the private dev target for local plugin-folder testing.

Plugin installation is separate from AirPrompter MCP authentication.
A successful package install does not prove authentication, connection
doctor, or live verifier success.
