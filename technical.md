---
id: technical
aliases: []
tags:
  - note-taking
date: "2024-07-17"
title: technical
---

# technical

## [[2025-01-19]] 

Help in formating (e.g. wiki-vim) in nvim lua: https://stackoverflow.com/questions/65549814/setting-vimwiki-list-in-a-lua-init-file -- to follow url links in nvim I seem to need the keybinding of wiki-vim (<return>)

## Foam [[2024-10-28-Monday]]

<https://foambubble.github.io/foam/>

<https://foambubble.github.io/foam/user/getting-started/recommended-extensions>

_a formidable list of capabilities_

**a very cool automatic github repository tool: <https://github.com/new?template_name=foam-template&template_owner=foambubble>**

## Notetaking with vscode: [[2024-10-28-Monday]]

notetaking with vscode: recommendations?

<https://www.reddit.com/r/Zettelkasten/comments/1044bb1/best_obsidianlike_extensions_for_vscode/>

Here are the suggestions rated for my particular use-case of finding something that feels most like Obsidian when typing and linking around:

Foam: So far the most like obsidian with wikilinks, the ability to like to sub-headings. Still not similar enough. When I do in-line views of headings (ie ![[link#heading]] it only shows to the next heading, even if it is a lower level. Obsidian shows lower-leveled headings which I prefer. Also in the case of non-unique headings Obsidian allows you to use a heading chain to refer to the specific one you want, ie ![[link#parent_heading#non_unique_heading]] This functionality is key to my usage.

Markdown Memo: If all you want is to add wikilinks to Obsidian and use the for automatic file-creation, without all of the graph generation fluff, this one is nice. It looks like it has better native tools for file structure flattening than Foam as well.

Dendron: Looks like a cool simple tool, not particularly similar to Obsidian. If I were to switch to Dendron for coding I would need to switch to it for everything. Not a total deal-breaker but not the first thing I'm going to try

## Explore "Notesnook"

[[2024-10-18-Friday]]
Has rich import options. I originally used it to import Keep files last year.

## [[1729251592-linux-commands|linux-commands]]

## Yazi file manager

<https://github.com/sxyazi/yazi>

### Keybindings

## Keybindings[](https://yazi-rs.github.io/docs/quick-start#keybindings "Direct link to Keybindings")

tip

For all keybindings, see the default keymap.toml file.

### Navigation[](https://yazi-rs.github.io/docs/quick-start#navigation "Direct link to Navigation")

To navigate between files and directories you can use the arrow keys ←, ↓, ↑ and → or Vim-like keys such as h, j, k, l:

| Key binding | Alternate key | Action                                          |
| ----------- | ------------- | ----------------------------------------------- |
| k           | ↑             | Move the cursor up                              |
| j           | ↓             | Move the cursor down                            |
| l           | →             | Enter hovered directory                         |
| h           | ←             | Leave the current directory and into its parent |

Further navigation commands can be found in the table below.

| Key binding | Action                           |
| ----------- | -------------------------------- |
| K           | Seek up 5 units in the preview   |
| J           | Seek down 5 units in the preview |
| g ⇒ g       | Move cursor to the top           |
| G           | Move cursor to the bottom        |

### Selection[](https://yazi-rs.github.io/docs/quick-start#selection "Direct link to Selection")

To select files and directories, the following commands are available.

| Key binding | Action                                     |
| ----------- | ------------------------------------------ |
| Space       | Toggle selection of hovered file/directory |
| v           | Enter visual mode (selection mode)         |
| V           | Enter visual mode (unset mode)             |
| Ctrl + a    | Select all files                           |
| Ctrl + r    | Inverse selection of all files             |
| Esc         | Cancel selection                           |

### File operations[](https://yazi-rs.github.io/docs/quick-start#file-operations "Direct link to File operations")

To interact with selected files/directories use any of the commands below.

| Key binding  | Action                                                                  |
| ------------ | ----------------------------------------------------------------------- |
| o            | Open selected files                                                     |
| O            | Open selected files interactively                                       |
| Enter        | Open selected files                                                     |
| Ctrl + Enter | Open selected files interactively (some terminals don't support it yet) |
| y            | Yank selected files (copy)                                              |
| x            | Yank selected files (cut)                                               |
| p            | Paste yanked files                                                      |
| P            | Paste yanked files (overwrite if the destination exists)                |
| \-           | Symlink the absolute path of yanked files                               |
| \_           | Symlink the relative path of yanked files                               |
| Ctrl + \-    | Hardlink yanked files                                                   |
| Y or X       | Cancel the yank status                                                  |
| d            | Trash selected files                                                    |
| D            | Permanently delete selected files                                       |
| a            | Create a file (ends with / for directories)                             |
| r            | Rename selected file(s)                                                 |
| ;            | Run a shell command                                                     |
| :            | Run a shell command (block until finishes)                              |
| .            | Toggle the visibility of hidden files                                   |
| z            | Jump to a directory using zoxide                                        |
| Z            | Jump to a directory or reveal a file using fzf                          |

### Copy paths[](https://yazi-rs.github.io/docs/quick-start#copy-paths "Direct link to Copy paths")

To copy paths, use any of the following commands below.

_Observation: c ⇒ d indicates pressing the c key followed by pressing the d key._

| Key binding | Action                              |
| ----------- | ----------------------------------- |
| c ⇒ c       | Copy the file path                  |
| c ⇒ d       | Copy the directory path             |
| c ⇒ f       | Copy the filename                   |
| c ⇒ n       | Copy the filename without extension |

### Filter files[](https://yazi-rs.github.io/docs/quick-start#filter-files "Direct link to Filter files")

| Key binding | Action       |
| ----------- | ------------ |
| f           | Filter files |

### Find files[](https://yazi-rs.github.io/docs/quick-start#find-files "Direct link to Find files")

| Key binding | Action                   |
| ----------- | ------------------------ |
| /           | Find next file           |
| ?           | Find previous file       |
| n           | Go to the next found     |
| N           | Go to the previous found |

### Search files[](https://yazi-rs.github.io/docs/quick-start#search-files "Direct link to Search files")

| Key binding | Action                                                                         |
| ----------- | ------------------------------------------------------------------------------ |
| s           | Search files by name using [fd](https://github.com/sharkdp/fd)                 |
| S           | Search files by content using [ripgrep](https://github.com/BurntSushi/ripgrep) |
| Ctrl + s    | Cancel the ongoing search                                                      |

### Sorting[](https://yazi-rs.github.io/docs/quick-start#sorting "Direct link to Sorting")

To sort files/directories use the following commands.

_Observation: , ⇒ a indicates pressing the , key followed by pressing the a key._

| Key binding | Action                           |
| ----------- | -------------------------------- |
| , ⇒ m       | Sort by modified time            |
| , ⇒ M       | Sort by modified time (reverse)  |
| , ⇒ c       | Sort by creation time            |
| , ⇒ C       | Sort by creation time (reverse)  |
| , ⇒ e       | Sort by file extension           |
| , ⇒ E       | Sort by file extension (reverse) |
| , ⇒ a       | Sort alphabetically              |
| , ⇒ A       | Sort alphabetically (reverse)    |
| , ⇒ n       | Sort naturally                   |
| , ⇒ N       | Sort naturally (reverse)         |
| , ⇒ s       | Sort by size                     |
| , ⇒ S       | Sort by size (reverse)           |
| , ⇒ r       | Sort randomly                    |

### Multi-tab[](https://yazi-rs.github.io/docs/quick-start#multi-tab "Direct link to Multi-tab")

| Key binding  | Action                             |
| ------------ | ---------------------------------- |
| t            | Create a new tab with CWD          |
| 1, 2, ..., 9 | Switch to the N-th tab             |
| \[           | Switch to the previous tab         |
| \]           | Switch to the next tab             |
| {            | Swap current tab with previous tab |
| }            | Swap current tab with next tab     |
| Ctrl + c     | Close the current tab              |

## Flavors[](https://yazi-rs.github.io/docs/quick-start#flavors "Direct link to Flavors")

Pick a color scheme you likehttps://github.com/igniteflow/terminator-keyboard-shortcuts from our [flavors repository](https://github.com/yazi-rs/flavors), or [cooking a flavor](https://yazi-rs.github.io/docs/flavors/overview#cooking)!

## linux

G

- [[vimrc-lenovo.md]]
- [[vimrc-lenovo-aug.md]]
- [[Guide to wiki.vim.md]]
- [[vimrc-lenovo-july.md]]
- [[vimrc-android]]
- [[vimrc-beelink-july.md]]
- [[pages/vimrc-beelink-9-2024]]
- [[vimrc-android]]
- [[Xresources-lenovo.md]]
- [[issues with wiki.md]]
- [[Install apk.md]]
- [[config.edn]]
- [[vimrc-beelink-july.md]]
- [[Zettelkasten method.md]]
- [[broken links output.md]]
- [[table memory sticks.md]]
- [[vimrc-android]]
- [[pages/vimrc-beelink-9-2024]]

## terminator [[2024-10-31-Thursday]]

<https://github.com/igniteflow/terminator-keyboard-shortcuts>
[./assets/elpedro_terminator.pdf](./assets/elpedro_terminator.pdf)

## rsync

The rsync syntax is really simple:

rsync [OPTIONS] SOURCE DESTINATION

Options
The following are some of the most useful options to add to the rsync command:

-v or --verbose: the verbose flag will display information about the progress of the task.
-a or --archive: equals -rlptgoD. The archive flag sets the most common options instead of setting them individually.
The following are the options set with -a that can also be set one by one:

-r or --recursive: recurses into directories. Must be used when you need to copy all the contents inside a directory.
-l or --links: copies symlinks as symlinks, does not copy the file to which they point to avoiding loopbacks to other directories.
-p or --perms: preserves the permission of the file.
-t or --times: preserves the original modification timestamps.
-g or --group: preserves the files' groups ownership.
-o or --owner: preservers the files' owners.
-D: preserves the device files and special files. You can use the options --devices and --specials to accomplish this.

## declaring wiki_root in nvim

[[journal/2024-12-18.md]]

It appears most things are working now in nvim with wiki.vim plugin

I had to hard wire set it in .local/share/nvim/lazy/wiki.vim/plugin/wiki.vim

## installed "tilix" and it seems to meet much of the criteria for a tiling terminal
