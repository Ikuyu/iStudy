# 1. ABOUT iSTUDY

iStudy — where the 'i' stands for individual (or I) — is a TUI study-aid dashboard. You decide what to learn and when to learn it. Flashcards are only marked as 'learned' when you say they are. With several study methods to choose from, you can pick the one that works best for you.

# 2. USAGE

1. Make sure you have a recent version of Ruby installed.
2. From the project folder, install the dependencies: `$ bundle install`.
3. Start the application from the project folder: `$ bundle exec ruby app.rb`. Alternatively, you can run: `$ ruby app.rb`.

# 3. IMPORTANT

1. iStudy has been tested in the following terminal emulators:

- iTerm2
- Ghostty.

iStudy cannot run in the default macOS Terminal app because it requires a modern terminal emulator. Its user interface is built with Ratatui Ruby, which provides Ruby bindings for Ratatui, a Rust-based TUI library.

2. To use Alt-V on macOS, configure the Option key as a Meta key in your terminal emulator.

- In Ghostty, add the following line to your configuration:  `macos-option-as-meta = left`
- In iTerm2, go to: **Settings → Profiles → Keys**. Then set `Left Option Key` to `Esc+`.


# 4. TEXT-EDITING KEYBOARD SHORTCUTS


## 4.1 Editing
Control-X: cut the selected text and copy it to the system clipboard.
Control-Y, Shift-Control-Z: redo (Shift-Ctrl-Z doesn't work in all terminals).
Control-Z: undo.
Control-T: swap the character behind the insertion point with the character in front of the insertion point.

## 4.2 Navigation
Control-F, Right Arrow: move one character forwards.
Control-B, Left Arrow: move one character backwards.

Fn-Up Arrow, Fn-Left Arrow, Option-Up Arrow, Control-A: move the insertion point to the beginning of the line.
Fn-Down Arrow, Fn-Right Arrow, Option-Down Arrow, Control-E: move the insertion point to the end of the line.

Option-Left Arrow: move the insertion point to the beginning of the previous word.
Option-Right Arrow: move the insertion point to the end of the next word.

Control-L: centre the insertion point in the text.

TAB, Control-P: next inputfield.
BACKTAB, Control-N: previous inputfield.

## 4.3 Removing Text

Ctrl-W, Option-Backspace: delete the word to the left of the insertion point.
Fn-Option-Backspace: delete the word to the right of the insertion point.
Control-H, Backspace: delete the character to the left of the insertion point.
Control-D, Fn-Backspace: delete the character to the right of the insertion point.
Control-K: delete text from the right of the insertion point to the end of the line.

## 4.4 Selecting Text

Control-A: select all text.

Shift-Control-F[^1], Shift-Right Arrow: extend text selection one character to the right.
Shift-Control-B[^1], Shift-Left Arrow: extend text selection one character to the left.

Option-Shift-Left Arrow: extend text selection to the beginning of the current word, then to the beginning of the following word if pressed again.
Option-Shift-Right Arrow: extend text selection to the end of the current word, then to the end of the following word if pressed again.

Shift-Up Arrow, Fn-Shift-Up Arrow[^1], Option-Shift-Up Arrow: extend text selection to the beginning of the line.
Shift-Down Arrow, Fn-Shift-Down Arrow[^1], Option-Shift-Down Arrow: extend text selection to the end of the line.

Shift+Control+L[^1]: extend the text selection to the centre of the text.

[^1]: This keyboard shortcut works by default in Ghostty. To enable it in iTerm2, import `istudy.itermkeymap` under **Settings → Profiles → Keys → Key Bindings → Presets…**.
