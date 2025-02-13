---
id: technology
aliases:
  - technology
tags:
  - technical
date: "2024-09-03"
title: technology
---

## Return to trying MkDocs

https://www.blimped.nl/creating-a-beautiful-documentation-site-with-mkdocs/#purpose

This gives the method for creating individual venv:  https://stackoverflow.com/questions/75608323/how-do-i-solve-error-externally-managed-environment-every-time-i-use-pip-3

setting up the my-venv in the working folder allowed me to pip install to this project.

Start server with: ```my-venv/bin/mkdocs serve```


## Hugo trials :technical:  [journal/2025-02-10.md](journal/2025-02-10.md) 
- https://gohugo.io/getting-started/external-learning-resources/

- https://www.youtube.com/watch?v=0GZxidrlaRM I finally got something in the server, by using the flag "-D", telling it to serve the Drafts. One blogger posted this: "As of this post, Hugo automatically creates a directory folder on the root list file. Nice! And one must use --buildDrafts with hugo server instead of -D" but the short version worked for me.

Using a different theme I evidently need to use the long version.

**also** @isaacgraphics1416
2 years ago
If anyone else is getting an error which says:
"execute of template failed at <.url>: can’t evaluate field url in type page.Page" 
It's because ".URL" is depreciated and won't work in modern installs.
You can fix it by changing {{.URL}} to {{.Permalink}}:> 
## Tue 03 Sep 2024

- Software: inserting date in .vimrc: :technology: [month](https://man7.org/linux/man-pages/man3/strftime.3.html "strftime(3) - Linux manual page")
- Figuring out my own method of doing this note-taking:

1. Using the journal page to link to a subject page
2. From there time-stamping items
   - allowing for sub-subject links
3. Can I begin using this wiki as my personal information gathering place that makes sense?

## technical - initial setup [initial testing](initial testing.md) :technical:

[2024journal](2024journal.md) effort to get template for journals [initial
testing.md](initial testing.md)

[/configs/current-lenovo-vimrc.md|/configs/current-lenovo-vimrc]]
[current-beelink-vimrc](current-beelink-vimrc.md)

## For beelink where tab doesn't work

[[Keymappings for Obsidian.nvim]]

## aliases

- (open with "gf") /home/dale/.bash_aliases

## [[Table mode for nvim]]   2024-10-15 Tue

## [[1729083227-obsidian-commands|Obsidian commands]]

- [[1729083227-obsidian-commands|Obsidian commands]] [[2024-10-16-Wednesday]]

## an example

- calling an obsidium-nvim command as keymapping: <https://stackoverflow.com/questions/78089195/map-obsidianextractnote-in-neovim>
- vim.keymap.set('x', '<leader>ox', ':ObsidianExtractNote<cr>')

## Links index

- [[1729012619-software.md]]

- [[vim tabular.md]]

## obsidian 1.8

[youtube](https://youtu.be/w44sNTl-zvI?si=1V0oYjhGr_G7qNpg)

especially web viewer
