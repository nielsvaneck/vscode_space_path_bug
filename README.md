# VSCode space path terminal link bug

Reproduction of the non-clickable links in VSCode due to spaces in paths issue reported here: https://github.com/microsoft/vscode/issues/97941

VSCode renders paths in its terminal as clickable links to resources. Sadly, these are not rendered as links or clickable when the path contains a space.

This repo contains two folders with a python program that divides by 0 to produce an error. One has a space in the path, the other does not.

Executing the code in the folder without the space results in VSCode rendering a clickable link in the terminal.

![Execution without space, link](images/cursor_over_path_without_space.png)

Executing the code in the folder with a space results in VSCode not rendering a clickable link.

![Execution without space, link](images/cursor_over_path_with_space.png)
