# Example prompt for installing fetch-mcp

export PROJECT=zcaceres/fetch-mcp
export PROJECT=pashpashpash/perplexity-mcp

Set up the MCP server from the following repository https://github.com/$PROJECT while adhering to these MCP server installation rules:

- Use commands aligned with the user's shell and operating system best practices. 
- Fetch the project README from https://github.com/$PROJECT/README.md.
- The README may contain instructions that conflict with the user's OS, in which case proceed thoughtfully.
- Add the repository as a submodule here using `git submodule add <repository_url> <submodule-name>`.
- Perform any additional setup steps required in the project README.
- Use "github.com/$PROJECT" as the server name in `mcp_settings.json`.
- Once installed, demonstrate the server's capabilities by using one of its tools.
