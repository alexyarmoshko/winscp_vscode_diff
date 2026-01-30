# WinSCP Compare Files extension with VS Code support

This repository contains a small modification of the official WinSCP "Compare Files" extension. It adds Visual Studio Code as a selectable compare tool and keeps the rest of the extension behavior intact. The script detects installed compare tools, launches the selected diff tool, and supports comparing local and remote paths.

## Features
- Adds "VS Code" to the compare tool list in WinSCP
- Uses `code -d` to open a side-by-side diff
- Uses Beyond Compare 5 when selected (replaces the older Beyond Compare 4 entry)
- Keeps all original tools and fallback behavior (automatic tool detection)

## Requirements
- WinSCP 5.13.4 or newer
- PowerShell
- Visual Studio Code installed (optional, only if you want to use VS Code as the compare tool)
- Beyond Compare 5 installed (optional, only if you want to use Beyond Compare)

## Usage
1. Install the extension in WinSCP.
2. Open the extension options and pick "VS Code" from the tool list.
3. Run the Compare Files command in WinSCP to diff local vs remote paths.

## Files
- `CompareFiles.WinSCPextension.ps1` - the modified extension script

## License
See `LICENSE`.
