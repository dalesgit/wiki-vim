---
title: common commands
date: 2024-07-10
tags: 
---

# common commands

`n`     [leader]ww          |[plug](wiki-index)|                 [GLOBAL] \
  `n`     [leader]wn          |[plug](wiki-open)|                  [GLOBAL] \
  `n`     [leader]w[leader]w  |[plug](wiki-journal)|               [GLOBAL] \
  `n`     [leader]wx          |[plug](wiki-reload)|                [GLOBAL] \
  `n`     [leader]wgb         |[plug](wiki-graph-find-backlinks)| \
  `n`     [leader]wgr         |[plug](wiki-graph-related)| \
  `n`     [leader]wgO         |[plug](wiki-graph-check-orphans)| \
  `n`     [leader]wgi         |[plug](wiki-graph-in)| \
  `n`     [leader]wgo         |[plug](wiki-graph-out)| \
  `n`     [leader]wd          |[plug](wiki-page-delete)| \
  `n`     [leader]wr          |[plug](wiki-page-rename)| \
  `n`     [leader]wp          |[plug](wiki-export)| \
  `n`     [leader]wsl         |[plug](wiki-tag-list)| \
  `n`     [leader]wss         |[plug](wiki-tag-search)| \
  `n`     [leader]wa          |[plug](wiki-link-add)| \
  `i`     [c-q]               |[plug](wiki-link-add)| \
  `n`     [tab]               |[plug](wiki-link-next)| \
  `n`     [s-tab]             |[plug](wiki-link-prev)| \
  `n`     [cr]                |[plug](wiki-link-follow)| \
  `n`     [c-w][cr]           |[plug](wiki-link-follow-split)| \
  `n`     [c-w][tab]          |[plug](wiki-link-follow-vsplit)| \
  `n`     [c-w]u              |[plug](wiki-link-follow-tab)| \
  `n`     [bs]                |[plug](wiki-link-return)| \
  `n`     gl                  |[plug](wiki-link-transform-operator)| \
  `x`     [cr]                |[plug](wiki-link-transform-visual)| \
  `n`     [M-p]               |[plug](wiki-journal-prev)|          [JOURNAL] \
  `n`     [M-n]               |[plug](wiki-journal-next)|          [JOURNAL] \
  `n`     [leader][c-n]       |[plug](wiki-journal-copy-tonext)|   [JOURNAL] \
  `n`     [leader]wu          |[plug](wiki-journal-toweek)|        [JOURNAL] \
  `n`     [leader]wm          |[plug](wiki-journal-tomonth)|       [JOURNAL] \
---

---
  [leader]wf       | transform link to another type
---

wiki-pages   | [C-g] \
Ctrlsf ==]   | [C-M-f] (folder) \
gm ==] LivedownToggle \

Zotero: \
    "@" part of auth/title then [C-x] [C-o]  \
    (leader) zi = info \
    (leader) za = all fields \

---

[C-M- +/-] size terminal font

---

- nmap     [C-S]f [Plug]CtrlSFPrompt
- vmap     [C-S]f [Plug]CtrlSFVwordPath
- vmap     [C-S]F [Plug]CtrlSFVwordExec
- nmap     [C-S]n [Plug]CtrlSFCwordPath
- nmap     [C-S]p [Plug]CtrlSFPwordPath
- nnoremap [C-S]o :CtrlSFOpen[CR]
- nnoremap [C-S]t :CtrlSFToggle[CR]
- inoremap [C-S]t [Esc]:CtrlSFToggle[CR]

"
nmap gm :LivedownToggle[CR]

"---
" insert date/time
map [leader]D :put =strftime('# %a %Y-%m-%d %H:%M:%S%z')[CR]  \
set foldlevelstart=99
"
---
The mappings that act on links are listed in |wiki-mappings-default|. The most
notable default mappings are:

- A link may be followed with `[cr]`.
- `[cr]` used on normal text (not on a link) will transform the text into
  a link of the type specified by |g:wiki_link_creation|. This also works in
  visual mode.
- Similarly, `gl` may be used to turn operated text into a link.
- One may use `[bs]` to navigate back after following a link.
- `[leader]wf` can be used to transform a link between different types (see
  |g:wiki_link_transforms|).

---
