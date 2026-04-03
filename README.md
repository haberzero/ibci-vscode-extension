# IBC-Inter VS Code Extension

This extension provides syntax highlighting and basic language support for IBC-Inter (`.ibci`) files in Visual Studio Code.

## Features

- Syntax highlighting for IBCI language constructs
- Support for LLM function blocks (`llm...llmend`)
- Intent marker highlighting (`@`, `@+`, `@!`)
- Behavior description highlighting (`@~...~`)
- Variable interpolation highlighting (`$variable`)
- Automatic bracket matching
- Basic indentation rules

## Installation

### From Source

1. Clone this repository
2. Copy the `ibci-vscode-extension` folder to your VS Code extensions directory:
   - **Windows**: `%USERPROFILE%\.vscode\extensions\`
   - **macOS**: `~/.vscode/extensions/`
   - **Linux**: `~/.vscode/extensions/`
3. Restart VS Code

### From GitHub Release

1. Download the `.vsix` file from the releases page
2. In VS Code, run `Extensions: Install from VSIX...` from the Command Palette (`Ctrl+Shift+P`)
3. Select the downloaded `.vsix` file

## Language Features

### Supported Constructs

| Construct | Example |
|-----------|---------|
| Control Flow | `if`, `elif`, `else`, `for`, `while`, `return` |
| LLM Keywords | `llm`, `llmend`, `__sys__`, `__user__`, `llmexcept`, `retry` |
| Intent Markers | `@`, `@+`, `@!`, `@-` |
| Behavior Block | `@~...~` |
| Types | `int`, `float`, `str`, `bool`, `list`, `dict` |
| Constants | `True`, `False`, `None` |
| Variable Reference | `$variable_name` |

## File Association

Files with the `.ibci` extension are automatically recognized as IBC-Inter files.

## Configuration

No additional configuration is required. The extension works out of the box with sensible defaults.

## Building

If you want to package this extension as a `.vsix` file:

1. Install `vsce` (VS Code Extension Manager):
   ```bash
   npm install -g @vscode/vsce
   ```

2. Package the extension:
   ```bash
   cd ibci-vscode-extension
   vsce package
   ```

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

## License

MIT License
