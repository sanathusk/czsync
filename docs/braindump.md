Tech stack:
bunjs script, bunjs needs to be installed for development, the binary distruction used for production with have bun runtime embeded so no need to install bunjs on production machine explictely.
dependencies:
 https://github.com/vadimdemedes/ink - TUI library 

the scripts follows following steps:
1. check if chezmoi is install ed on the machine, if not display message like "The tool works in conjection with chezmoi,please ensure that chezmoi is installed and is added to path"
2. run `chezmoi status` command and stores that output in a map where the path of the file is key and value is the status code.
3.Open a two pane layout using ink(https://github.com/vadimdemedes/ink) , left panel is the primary panel where the user will see the list of files and user should be able to select the file and a preview of the file content would be display in the pane on the right,something like an output of cat command
