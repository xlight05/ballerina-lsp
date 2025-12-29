# Ballerina LSP Plugin for Claude Code

This plugin provides Language Server Protocol (LSP) support for the Ballerina programming language in Claude Code. With this plugin, Claude Code gains deep understanding of Ballerina code through real-time language server integration.

## Features

With this plugin, Claude Code provides enhanced support for Ballerina files:

- **Instant diagnostics**: Syntax errors, type errors, and warnings appear immediately after edits
- **Code navigation**: Go to definition, find references, and hover information for symbols
- **Type information**: Access detailed type information and documentation for Ballerina constructs
- **Code intelligence**: Full access to Ballerina's semantic understanding of your code
- **Symbol navigation**: Browse and search for functions, services, records, and other Ballerina constructs

## Prerequisites

This plugin requires the Ballerina language distribution to be installed on your machine.

**Minimum Requirements:**
- Ballerina >= 2201.12.0 (Swan Lake Update 12 or later)
- The `bal` command must be available in your system PATH
- Java 21 (bundled with Ballerina distribution)

### Installing Ballerina

1. Download and install Ballerina from [https://ballerina.io/downloads/](https://ballerina.io/downloads/)
2. Follow the installation instructions for your platform (macOS, Linux, or Windows)
3. Verify the installation:
   ```bash
   bal version
   ```

You should see output similar to:
```
Ballerina 2201.13.1 (Swan Lake Update 13)
Language specification 2024R1
Update Tool 1.5.1
```

**Verify Installation:**
```bash
# Check Ballerina is in PATH
bal version

# Check Ballerina home
bal home
```

## Installation

### From Claude Code Marketplace

You can install this plugin directly from the Claude Code marketplace:
- Open Claude Code
- Go to `/plugins` > `Marketplaces` > `Add Marketplace`
- Paste `https://github.com/xlight05/ballerina-lsp` and enter: 
- Click on Browse Plugins
- Click on ballerina-lsp
- Install based on the permission scope you require.


### Manual Installation (Development)

For development or testing, you can install the plugin locally:

1. Clone or download this repository:
   ```bash
   git clone https://github.com/xlight05/ballerina-lsp.git
   ```
2. Install the plugin:
   ```bash
   claude install /path/to/ballerina-lsp
   ```

Or start Claude Code with the plugin directory:
   ```bash
   claude --plugin-dir /path/to/ballerina-lsp
   ```

## Usage

Once installed, the plugin automatically activates when you work with Ballerina files (`.bal` extensions).

### Supported File Types

- `.bal` - Ballerina source files
