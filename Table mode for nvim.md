---
id: Table mode for nvim
aliases: []
tags: []
---

## Table mode for nvim

- <https://github.com/SCJangra/table-nvim>
  default configs
  {
  padd_column_separators = true, -- Insert a space around column separators.
  mappings = { -- next and prev work in Normal and Insert mode. All other mappings work in Normal mode.
  next = '<TAB>', -- Go to next cell.
  prev = '<S-TAB>', -- Go to previous cell.
  insert_row_up = '<A-k>', -- Insert a row above the current row.
  insert_row_down = '<A-j>', -- Insert a row below the current row.
  move_row_up = '<A-S-k>', -- Move the current row up.
  move_row_down = '<A-S-j>', -- Move the current row down.
  insert_column_left = '<A-h>', -- Insert a column to the left of current column.
  insert_column_right = '<A-l>', -- Insert a column to the right of current column.
  move_column_left = '<A-S-h>', -- Move the current column to the left.
  move_column_right = '<A-S-l>', -- Move the current column to the right.
  insert_table = '<A-t>', -- Insert a new table.
  insert_table_alt = '<A-S-t>', -- Insert a new table that is not surrounded by pipes.
  delete_column = '<A-d>', -- Delete the column under cursor.
  }
  }
  I removed 2024-10-18 Fri to see if I can get Obsidian to read tables better. It didn't work. Replaced.

  ## 2024-10-15 Tue

  ### Working on markdown in nvim

  1. folding looks and works smoothly
  2. bold and _emphasis_ (**italic**) works with visual mode
  3. table mode is simple but elegant cf. above
  4. insert template is easy -- "ObsidianTemplate"