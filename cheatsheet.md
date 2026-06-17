# ⚡ WebStorm to Neovim + Cmux Master Cheatsheet

## 🏃 Basic Vim Motions (Moving Around)
| Key | Action |
| :--- | :--- |
| `h` / `j` / `k` / `l` | Left / Down / Up / Right |
| `gg` / `G` | Jump to the very top / very bottom of file |
| `0` / `^` / `$` | Jump to start of line / first character / end of line |
| `Ctrl+d` / `Ctrl+u` | Scroll Down half-page / Scroll Up half-page |
| `%` | Jump to matching bracket/parenthesis |
| `o` / `O` | Insert new line below / above current line |

## 📝 Words & Fast Editing (Vim Grammar)
| Key | Action |
| :--- | :--- |
| `w` / `b` / `e` | Jump forward a word / backward a word / to end of word |
| `ciw` | **Change Inner Word** (Deletes word under cursor, enters Insert mode) |
| `diw` | **Delete Inner Word** (Deletes word under cursor) |
| `yiw` | **Yank Inner Word** (Copies word under cursor) |
| `dd` / `yy` | Delete (cut) entire line / Yank (copy) entire line |
| `p` / `P` | Paste after cursor / Paste before cursor |
| `u` / `Ctrl+r` | Undo / Redo |
| `x` | Delete character under cursor |

## 🔍 Search, Files & LazyVim Essentials
| Key | Action |
| :--- | :--- |
| `<leader><space>` | Find Files (Search by filename) |
| `<leader>/` | Grep (Search for text inside all files) |
| `<leader>e` | Toggle Neo-tree (File explorer sidebar) |
| `<leader>w` | Save current file |
| `<leader>qq` | Quit Neovim completely |
| `]b` / `[b` | Switch to next / previous open buffer (tab) |
| `<leader>bd` | Close current buffer (keeps window open) |
| `<leader>sk` | Search Keymaps (Find any forgotten shortcut!) |
| `<leader>cm` | Open Mason (Install LSPs, linters, formatters) |

## 🧠 Code Navigation & Refactoring (LSP)
| Key | Action |
| :--- | :--- |
| `K` | Hover Docs (Types, parameters, signatures) |
| `gd` | Go to Definition |
| `gr` | Go to References (Project-wide usages) |
| `gI` | Go to Implementation |
| `<leader>cr` | Rename variable/function across the entire project |
| `<leader>ca` | Code Action (Quick fixes, auto-imports) |
| `]d` / `[d` | Jump to next / previous code error or warning |

## 🖥️ Layout & Windows (Cmux + Neovim)
| Key | Action |
| :--- | :--- |
| `Cmd+Opt+Arrows` | **Cmux:** Move focus between Claude, Nvim, Terminal |
| `Cmd+Shift+[` / `]` | **Cmux:** Cycle through your left-sidebar workspaces |
| `Cmd+w` | **Cmux:** Close current cmux pane/window |
| `Ctrl+w` + `h/j/k/l` | **Nvim:** Move focus between internal splits |
| `Ctrl+w` + `v` | **Nvim:** Split window vertically |
| `Ctrl+w` + `s` | **Nvim:** Split window horizontally |
| `Ctrl+w` + `=` | **Nvim:** Make all splits exactly equal size |
| `Ctrl+w` + `q` | **Nvim:** Close current Neovim split |

## 🤖 AI (Supermaven)
| Key | Action |
| :--- | :--- |
| `<M-l>` | Accept full suggestion (Ghost text) |
| `<M-j>` | Accept suggestion word-by-word |
| `<M-]>` | Clear current suggestion |
| `Ctrl+e` | Close standard autocomplete menu (if blocking) |

## 🔄 Git Diffs (`diffview.nvim`)
| Key | Action |
| :--- | :--- |
| `<leader>gD` | Open Diffview (WebStorm side-by-side commit view) |
| `<leader>gC` | Close Diffview |
| `zR` / `zM` | Unfold full file / Fold unchanged lines |
| `]c` / `[c` | Jump to next / previous changed code block |
| `s` / `u` | Stage / Unstage highlighted file (in bottom panel) |
| `X` | Discard all changes in highlighted file |

## 🚀 Git Workspace (LazyGit: `<leader>gg`)
| Key | Action |
| :--- | :--- |
| `1`-`5` | Switch panels (Status, Files, Branches, Commits) |
| `Space` | Toggle stage (Files) OR Checkout (Branches) |
| `a` | Stage ALL modified files |
| `c` | Quick inline commit |
| `C` | Commit using Neovim editor (Loads your PR template) |
| `P` | Push commits to origin |
| `n` | Create new branch |
| `o` | Open PR in web browser |
| `q` | Quit LazyGit |

## 🐙 GitHub PR Reviews (`octo.nvim`)
| Command / Key | Action |
| :--- | :--- |
| `<leader>gp` | List open PRs to review |
| `:Octo review start` | Start draft review (Opens Diffview comparison) |
| `\ca` | Add Comment to line (While looking at PR diff) |
| `:Octo review resume`| Re-open accidentally closed review diff |
| `:Octo review discard`| Delete draft review (Fixes "pending review" error) |
| `:Octo review submit` | Finalize review (Approve/Comment/Request) |
