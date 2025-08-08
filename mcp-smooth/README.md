# mcp-smooth

[![smithery badge](https://smithery.ai/badge/@csrdltte/mcp-smooth)](https://smithery.ai/server/@csrdltte/mcp-smooth)


### Usage with VS Code

For quick installation, use one of the one-click install buttons below:

[![Install with NPX in VS Code](https://img.shields.io/badge/VS_Code-NPM-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://insiders.vscode.dev/redirect/mcp/install?name=mcp-smooth&config=%7B%22command%22%3A%22npx%22%2C%22args%22%3A%5B%22-y%22%2C%22mcp-smooth%22%5D%7D)

For manual installation, add the following JSON block to your User Settings (JSON) file in VS Code. You can do this by pressing `Ctrl + Shift + P` and typing `Preferences: Open User Settings (JSON)`.

Optionally, you can add it to a file called `.vscode/mcp.json` in your workspace. This will allow you to share the configuration with others.

> Note that the `mcp` key is not needed in the `.vscode/mcp.json` file.

```json
{
  "mcp": {
    "inputs": [
      {
        "type": "promptString",
        "id": "vaultPath",
        "description": "Path to Obsidian vault"
      }
    ],
    "servers": {
      "obsidian": {
        "command": "npx",
        "args": ["-y", "mcp-smooth", "${input:vaultPath}"]
      }
    }
  }
}
```