---
title: common commands
date: 2024-07-10
tags: 
---


*Contents*
* [common commands](#common commands)
* [table creation:](#table creation:)
    * [surround.vim](#table creation:#surround.vim)
* [digraphs https://vimhelp.org/digraph.txt.html](#digraphs https://vimhelp.org/digraph.txt.html)
* [[Vim Cheat Sheet](https://vim.rtorr.com/)](#digraphs https://vimhelp.org/digraph.txt.html#[Vim Cheat Sheet](https://vim.rtorr.com/))

## common commands
`n`     <leader>ww          |<plug>(wiki-index)|                 [GLOBAL] \
  `n`     <leader>wn          |<plug>(wiki-open)|                  [GLOBAL] \
  `n`     <leader>w<leader>w  |<plug>(wiki-journal)|               [GLOBAL] \
  `n`     <leader>wx          |<plug>(wiki-reload)|                [GLOBAL] \
  `n`     <leader>wgb         |<plug>(wiki-graph-find-backlinks)| \
  `n`     <leader>wgr         |<plug>(wiki-graph-related)| \
  `n`     <leader>wgc         |<plug>(wiki-graph-check-links)| \
  `n`     <leader>wgC         |<plug>(wiki-graph-check-links-g)| \
  `n`     <leader>wgO         |<plug>(wiki-graph-check-orphans)| \
  `n`     <leader>wgi         |<plug>(wiki-graph-in)| \
  `n`     <leader>wgo         |<plug>(wiki-graph-out)| \
  `n`     <leader>wf          |<plug>(wiki-link-transform)| \
  `n`     <leader>wd          |<plug>(wiki-page-delete)| \
  `n`     <leader>wr          |<plug>(wiki-page-rename)| \
  `n`     <leader>wt          |<plug>(wiki-toc-generate)| \
  `n`     <leader>wT          |<plug>(wiki-toc-generate-local)| \
  `n`     <leader>wp          |<plug>(wiki-export)| \
  `x`     <leader>wp          |<plug>(wiki-export)| \
  `n`     <leader>wll         |<plug>(wiki-link-show)| \
  `n`     <leader>wlh         |<plug>(wiki-link-extract-header)| \
  `x`     <leader>wlh         |<plug>(wiki-link-extract-header)| \
  `n`     <leader>wli         |<plug>(wiki-link-incoming-toggle)| \
  `n`     <leader>wlI         |<plug>(wiki-link-incoming-hover)| \
  `n`     <leader>wsl         |<plug>(wiki-tag-list)| \
  `n`     <leader>wsr         |<plug>(wiki-tag-reload)| \
  `n`     <leader>wsn         |<plug>(wiki-tag-rename)| \
  `n`     <leader>wss         |<plug>(wiki-tag-search)| \
  `n`     <leader>wa          |<plug>(wiki-link-add)| \
  `i`     <c-q>               |<plug>(wiki-link-add)| \
  `n`     <tab>               |<plug>(wiki-link-next)| \
  `n`     <s-tab>             |<plug>(wiki-link-prev)| \
  `n`     <cr>                |<plug>(wiki-link-follow)| \
  `n`     <c-w><cr>           |<plug>(wiki-link-follow-split)| \
  `n`     <c-w><tab>          |<plug>(wiki-link-follow-vsplit)| \
  `n`     <c-w>u              |<plug>(wiki-link-follow-tab)| \
  `n`     <bs>                |<plug>(wiki-link-return)| \
  `n`     gl                  |<plug>(wiki-link-transform-operator)| \
  `x`     <cr>                |<plug>(wiki-link-transform-visual)| \
  `ox`    au                  |<plug>(wiki-au)| \
  `ox`    iu                  |<plug>(wiki-iu)| \
  `ox`    at                  |<plug>(wiki-at)| \
  `ox`    it                  |<plug>(wiki-it)| \
  `n`     <c-p>               |<plug>(wiki-journal-prev)|          [JOURNAL] \
  `n`     <c-n>               |<plug>(wiki-journal-next)|          [JOURNAL] \
  `n`     <leader><c-n>       |<plug>(wiki-journal-copy-tonext)|   [JOURNAL] \
  `n`     <leader>wu          |<plug>(wiki-journal-toweek)|        [JOURNAL] \
  `n`     <leader>wm          |<plug>(wiki-journal-tomonth)|       [JOURNAL] \

  ---


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

## size terminal font
[C-M- +/-] size terminal font

---
## CtrlSF
- nmap     [C-S]f [Plug]CtrlSFPrompt
- vmap     [C-S]f [Plug]CtrlSFVwordPath
- vmap     [C-S]F [Plug]CtrlSFVwordExec
- nmap     [C-S]n [Plug]CtrlSFCwordPath
- nmap     [C-S]p [Plug]CtrlSFPwordPath
- nnoremap [C-S]o :CtrlSFOpen[CR]
- nnoremap [C-S]t :CtrlSFToggle[CR]
- inoremap [C-S]t [Esc]:CtrlSFToggle[CR]

"
## Livedown
nmap gm :LivedownToggle[CR]

"---

## insert date/time
map [leader]D :put =strftime('# %a %Y-%m-%d %H:%M:%S%z')[CR]  \
set foldlevelstart=99
"
---
## some notable default mappings
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


## table creation:

Creating table on-the-fly

To start using the plugin in the on-the-fly mode use :TableModeToggle mapped to <Leader>tm by default (which means \ t m if you didn't override the by :let mapleader = ',' to have , t m).

Tip: You can use the following to quickly enable / disable table mode in insert mode by using || or __:

function! s:isAtStartOfLine(mapping)
  let text_before_cursor = getline('.')[0 : col('.')-1]
  let mapping_pattern = '\V' . escape(a:mapping, '\')
  let comment_pattern = '\V' . escape(substitute(&l:commentstring, '%s.*$', '', ''), '\')
  return (text_before_cursor =~? '^' . ('\v(' . comment_pattern . '\v)?') . '\s*\v' . mapping_pattern . '\v$')
endfunction

inoreabbrev <expr> <bar><bar>
          \ <SID>isAtStartOfLine('\|\|') ?
          \ '<c-o>:TableModeEnable<cr><bar><space><bar><left><left>' : '<bar><bar>'
inoreabbrev <expr> __
          \ <SID>isAtStartOfLine('__') ?
          \ '<c-o>:silent! TableModeDisable<cr>' : '__'
Enter the first line, delimiting columns by the | symbol. The plugin reacts by inserting spaces between the text and the separator if you omit them:?

## surround.vim
c+s key key = change surround
d+s key = delete surround
y+s (e.g. 2w) key = insert

## digraphs https://vimhelp.org/digraph.txt.html

<C-k> ., = ellipsis
<C-k> 12 = one half (14 = fourth)
Rg = registered sign
Co = copyright
/- = dagger
/= = double dagger
co = care of sign
[all kinds of fractions]


## word count
press g then Ctrl-g

## add a word to spelling list
To add words to Vim's spell file, you can use the following commands:
zg: Adds the word under the cursor to the spell file
zw: Marks the word under the cursor as a misspelled word

## [Vim Cheat Sheet](https://vim.rtorr.com/)

## move lines
nmap <C-UP> :m-2<CR>  
nmap <C-DOWN> :m+1<CR>

## zotcite 

If you have installed `cmp-zotcite`, then, in Insert mode, type the `@` letter and one or more letters of either the last name of the first author or the reference title. The matching of citation keys is case-insensitive.

In Vim's Normal mode, put the cursor over a citation key and press:

- <Leader>zo to open the reference's attachment as registered in Zotero's database.
- <Leader>zi to see in the status bar the last name of all authors, the year, and the title of the reference.
- <Leader>za to see all fields of a reference as stored by Zotcite.
- <leader>zb to insert the abstract (if available) into the current buffer.
- <Leader>zy to see how the reference will be converted into YAML.
- <Leader>zv to view the (pdf or html) document generated from the current (Markdown, Rmd, or Quarto) document.

