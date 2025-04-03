# My MCP Servers

This repository manages various MCP (Model Context Protocol) server projects using Git submodules.

## Adding a New MCP Server Submodule

To add a new MCP server project as a submodule, use the following command:

```bash
git submodule add <repository_url> path/to/submodule
```

Replace `<repository_url>` with the URL of the MCP server's Git repository and `path/to/submodule` with the desired local directory path for the submodule (e.g., `servers/weather-server`).

After adding the submodule, commit the changes:

```bash
git commit -am "Add <server_name> submodule"
```

## Updating MCP Server Submodules

To pull the latest changes from the upstream repository for a specific submodule:

1.  Navigate to the submodule's directory:
    ```bash
    cd path/to/submodule
    ```
2.  Checkout the desired branch (usually `main` or `master`):
    ```bash
    git checkout main # or master
    ```
3.  Pull the latest changes:
    ```bash
    git pull origin main # or master
    ```
4.  Navigate back to the main project root:
    ```bash
    cd ../.. # Adjust path as necessary
    ```
5.  Stage the updated submodule reference:
    ```bash
    git add path/to/submodule
    ```
6.  Commit the update:
    ```bash
    git commit -m "Update <server_name> submodule"
    ```

To update *all* submodules to the latest commit on their respective tracked branches:

```bash
git submodule update --remote --merge
```

Then, commit the changes:

```bash
git commit -am "Update all submodules"
```

## Oddities

The perplexity mcp uses better-sqlite3 which seems to cause a lot of issues with pnpm, use npm and things should be fine.
