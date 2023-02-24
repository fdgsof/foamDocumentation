# Software
## Text editor, IDE and overall command center
Visual Studio Code (or short VS Code) is the best solution for all needs in terms of text editing and preparation of simulations. Extremely flexible also through the add-ins. Advantages are (not a complete list):
- tabbed editor
- nice search-and-replace function also over multiple files
- Can be a full IDE through extensions 
- Remote management through SSH plugin
- GIt integration
- Debugging tools
- syntax highlighting
- Workspaces (open multiple directories at once)
- Extensive theming and customization options

## SSH Tools
To access remote machines (such as a cluster or a local high performance machine), SSH will be useful.

### MobaXTerm
For an integrated beginner-friendly solution, MobaXTerm is great. File management, multiple terminal tabs, X-Window support. Free versions available (and also a portable version, so no installation required)
https://mobaxterm.mobatek.net/

### Windows Terminal
Windows terminal is a Microsoft product (free), which has tabbed terminal tabs. SSH does not require Putty or something like that anymore, but can be executed directly from a powershell window

### Putty
Not really required anymore, as Powershell supports the SSH command.

### WinSCP
Utility to transfer files. Might be useful in some cases, but files can also be transfered through SSH with VS Code or directly from powershell with `scp` .
