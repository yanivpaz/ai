# LSP / Language Server Protocol

`LSP` stands for `Language Server Protocol`.

It is a standard way for editors, IDEs, and coding tools to communicate with language-specific servers that provide code intelligence.

Common LSP-powered features include:
- autocomplete
- go-to-definition
- find references
- rename symbol
- hover documentation
- diagnostics and errors
- document and workspace symbols
- formatting

Why it matters:
- one language server can support many editors
- tooling logic stays in the server instead of being reimplemented per editor
- coding agents can use the same semantic code-navigation layer as human developers

Common LSP servers:
- `typescript-language-server` for TypeScript and JavaScript
- `pyright` for Python
- `gopls` for Go
- `rust-analyzer` for Rust
- `ruby-lsp` for Ruby
- `omnisharp` for C#

LSP vs MCP:
- `LSP` is for language-aware code intelligence inside source code
- `MCP` is for exposing external tools, services, data sources, and workflows to an agent

In agent workflows, `LSP` helps the model understand code structure more precisely, while `MCP` helps it act outside the editor.
