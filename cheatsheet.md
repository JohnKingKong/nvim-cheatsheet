<!-- To sync to site: cp ~/cheatsheet.md ~/nvim-cheatsheet/cheatsheet.md && cd ~/nvim-cheatsheet && git add cheatsheet.md && git commit -m "chore: sync cheatsheet.md" && git push -->

# ⚡ WebStorm to Neovim + Cmux Master Cheatsheet

## 🏃 Basic Vim Motions (Moving Around)

| Key | Action |
| :--- | :--- |
| `h` / `j` / `k` / `l` | Left / Down / Up / Right |
| `gg` / `G` | Jump to the very top / very bottom of file |
| `0` / `^` / `$` | Jump to start of line / first character / end of line |
| `Ctrl+d` / `Ctrl+u` | Scroll Down half-page / Scroll Up half-page |
| `%` | Jump to matching bracket, brace, or parenthesis |
| `o` / `O` | Insert new line below / above current line and enter Insert Mode |
| `<lineNb>gg` or `G` | Go directly to specific line number |
| `zz` / `zt` / `zb` | Center current line / Top of screen / Bottom of screen |
| `H` / `M` / `L` | Move cursor to High / Middle / Low positions of current viewport |

## 📝 Words & Fast Editing (Vim Grammar)

| Key | Action |
| :--- | :--- |
| `w` / `b` / `e` | Jump forward a word / backward a word / to end of word |
| `W` / `B` / `E` | Jump forward/backward/end of space-separated WORD |
| `ciw` | **Change Inner Word** (Deletes word under cursor, enters Insert mode) |
| `diw` | **Delete Inner Word** (Deletes word under cursor) |
| `yiw` | **Yank Inner Word** (Copies word under cursor without whitespace) |
| `viw` | **Visual Select Inner Word** (Selects word under cursor) |
| `vi"` / `vi{` / `vi[` | Visual Select inside quotes, curly braces, or brackets |
| `va"` / `va{` / `va[` | Visual Select around quotes, curly braces, or brackets (includes markers) |
| `ci"` / `ci{` / `ci[` | Change inside quotes, curly braces, or brackets (instantly clears block) |
| `di"` / `di{` / `di[` | Delete inside quotes, curly braces, or brackets |
| `daw` | **Delete a Word** (Deletes a word under cursor plus trailing whitespace) |
| `dd` / `yy` | Delete (cut) entire line / Yank (copy) entire line |
| `p` / `P` | Paste after cursor / Paste before cursor |
| `u` / `Ctrl+r` | Undo / Redo |
| `x` / `X` | Delete character under cursor / Delete character before cursor |
| `.` | **Repeat** the last modifying editing action |

## 🔍 Search, Files & LazyVim Essentials

| Key | Action |
| :--- | :--- |
| `<leader><space>` | Find Files (Fuzzy search by filename) |
| `<leader>/` | Live Grep (Search for text tokens inside all workspace files) |
| `<leader>e` | Toggle Neo-tree (File explorer sidebar tree view) |
| `<leader>w` | Save current file buffer changes |
| `<leader>qq` | Quit Neovim cleanly completely |
| `]b` / `[b` | Switch to next / previous open buffer tab |
| `<leader>bd` | Close current buffer (keeps active window layout intact) |
| `<leader>sk` | Search Keymaps (Find any missing shortcut interactively!) |
| `<leader>cm` | Open Mason setup manager (LSPs, linters, formatters) |
| `/`\<word\> | Search forward for matching text occurrences inside current file |
| `?`\<word\> | Search backward for matching text occurrences inside current file |
| `n` / `N` | Cycle forward / backward through active search matches |
| `:noh` | Clear active search visual highlighting masks |

## 🧠 Code Navigation & Refactoring (LSP)

| Key | Action |
| :--- | :--- |
| `K` | Hover Docs (Inspect engine types, parameters, parameters) |
| `gd` | Go to Definition |
| `gr` | Go to References (Find usages project-wide) |
| `gI` | Go to Implementation |
| `gy` | Go to Type Definition |
| `<leader>cr` | Rename variable/function symbol safely across entire project |
| `<leader>ca` | Code Action (Triggers quick-fixes, automatic imports, fixes) |
| `]d` / `[d` | Jump to next / previous code syntax error or warning flag |

## 🖥️ Layout & Windows (Cmux + Neovim)

| Key | Action |
| :--- | :--- |
| `Cmd+Opt+Arrows` | **Cmux:** Move focus directionally between panels |
| `Cmd+Shift+[` / `]` | **Cmux:** Cycle through left-sidebar system workspaces |
| `Cmd+w` | **Cmux:** Close current focused split/window tab |
| `Cmd+D` | **Cmux:** Split current screen window horizontally |
| `Cmd+Shift+D` | **Cmux:** Split current screen window vertically |
| `Cmd+Ctrl+Arrows` | **Cmux:** Resize size profiles of current active window partition |
| `Cmd+Ctrl+=` | **Cmux:** Balance all open cmux window partitions to equal sizes |
| `Cmd+Shift+Enter` | **Cmux:** Toggle Maximize/Zoom focus profile on current partition |
| `Ctrl+w` + `h/j/k/l` | **Nvim:** Move directional focus between internal code windows |
| `Ctrl+w` + `v` | **Nvim:** Create a vertical code window split |
| `Ctrl+w` + `s` | **Nvim:** Create a horizontal code window split |
| `Ctrl+w` + `=` | **Nvim:** Force all internal splits to balanced equal sizing scales |
| `Ctrl+w` + `q` | **Nvim:** Close current internal Neovim split pane |

## 🤖 AI Core Integrations

| Key | Action |
| :--- | :--- |
| `<M-l>` | **Supermaven:** Accept full inline code generation suggestions |
| `<M-j>` | **Supermaven:** Accept ghost text suggestions word-by-word |
| `<M-]>` | **Supermaven:** Clear/dismiss active predictive suggestions |
| `Ctrl+e` | Dismiss local completion popup lists when blocking ghost lines |
| `<leader>ca` | **Claude-Reviewer:** Approve intercepted Claude Code diff edits |
| `<leader>cd` | **Claude-Reviewer:** Reject/Abort intercepted Claude Code modifications |

## 🔄 Git Tools & Diffs

| Key | Action |
| :--- | :--- |
| `<leader>gD` | **Diffview:** Open comprehensive side-by-side Git workspace tree index |
| `<leader>gC` | **Diffview:** Close workspace comparison layout environment |
| `zR` / `zM` | Expand all structural folds / Collapse all folds to hide unchanged zones |
| `]c` / `[c` | Jump directly to next / previous modified line code hunks |
| `s` / `u` | Stage / Unstage current highlighted file targets (inside git console trees) |
| `X` | Discard all tracked modifications safely inside target file bounds |

## 🐙 GitHub PR Reviews (`octo.nvim`)

| Key / Command | Action |
| :--- | :--- |
| `<leader>gp` | Open query panel selector listing global pending open repository PR lines |
| `:Octo review start` | Initialize pull request design draft sequence comparisons |
| `\ca` | Inject structural context comments into lines within PR diff files |
| `:Octo review resume` | Re-open localized pull preview spaces when window crashes |
| `:Octo review discard` | Safely clear active review loops when sync processes hang |
| `:Octo review submit` | Deliver formal execution findings (Approve, Comment, Changes Request) |
