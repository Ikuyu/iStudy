# 1. ABOUT iSTUDY

iStudy — where the 'i' stands for individual (or I) — is a TUI dashboard study-aid. You decide what to learn and when to learn it. Flashcards are only marked as 'learned' when you say they are. With several study methods to choose from, you can pick the one that works best for you.

# 2. USAGE

1. Make sure you have a recent version of Ruby installed.
2. From the project folder, install the dependencies: `$ bundle install`.
3. Start the application from the project folder: `$ bundle exec ruby app.rb`. Alternatively, you can run: `$ ruby app.rb`.

# 3. IMPORTANT

1. iStudy has been tested in the following terminal emulators:

- iTerm2
- Ghostty.

It cannot run in the default macOS Terminal app because it requires a modern terminal emulator. Its user interface is built with Ratatui Ruby, which provides Ruby bindings for Ratatui, a Rust-based TUI library.

2. To use Alt-V on macOS, configure the Option key as a Meta key in your terminal emulator.

- In Ghostty, add the following line to your configuration:  `macos-⌥as-meta = left`
- In iTerm2, go to: **Settings → Profiles → Keys**. Then set `Left Option Key` to `Esc+`.

In iTerm2, the usual macOS keyboard shortcuts also work when iStudy.itermkeymap is imported via **Settings → Profiles → Keys → Key Bindings → Presets…**. Ghostty may also support these key combinations; however, this has not yet been tested.

# 4. Keyboard Shortcuts for Input Fields

## 4.1 Editing

| Shortcut | Action |
|---|---|
| `^x` | Cut the selected text and copy it to the system clipboard. |
| `^y`, `^⇧Z`[^1] | Redo (`^⇧z` doesn't work in all terminals). |
| `^z` | Undo. |
| `^t` | Swap the character behind the insertion point with the character in front of it. |

## 4.2 Navigation

| Shortcut | Action |
|---|---|
| `^f`, `→` | Move one character forwards. |
| `^b`, `←` | Move one character backwards. |
| `Fn↑`, `Fn←`, `⌥↑`, `^a` | Move the insertion point to the beginning of the line. |
| `Fn↓`, `Fn→`, `⌥↓`, `^e` | Move the insertion point to the end of the line. |
| `⌥←` | Move the insertion point to the beginning of the previous word. |
| `⌥→` | Move the insertion point to the end of the next word. |
| `^l` | Centre the insertion point in the text. |
| `TAB`, `^p` | Move to the next input field. |
| `BACKTAB`, `^n` | Move to the previous input field. |

## 4.3 Removing Text

| Shortcut | Action |
|---|---|
| `^w`, `⌥⌫` | Delete the word to the left of the insertion point. |
| `Fn⌥⌫` | Delete the word to the right of the insertion point. |
| `^h`, `⌫` | Delete the character to the left of the insertion point. |
| `^d`, `Fn⌫` | Delete the character to the right of the insertion point. |
| `^k` | Delete the text from the insertion point to the end of the line. |
| `^u` | Delete the text from the insertion point to the beginning of the line. |

## 4.4 Selecting Text

| Shortcut | Action |
|---|---|
| `^⇧a` | Select all text. |
| `^⇧f`, `⇧→` | Extend the selection one character to the right. |
| `^⇧b`, `⇧←` | Extend the selection one character to the left. |
| `⌥⇧←` | Extend the selection to the beginning of the current word. Press again to extend it to the beginning of the previous word. |
| `⌥⇧→` | Extend the selection to the end of the current word. Press again to extend it to the end of the next word. |
| `⇧↑`, `Fn⇧↑`, `⌥⇧↑` | Extend the selection to the beginning of the line. |
| `⇧↓`, `Fn⇧↓`, `⌥⇧↓` | Extend the selection to the end of the line. |
| `^⇧l` | Extend the selection to the centre of the text. |

[^1]: This keyboard shortcut works by default in Ghostty. To enable it in iTerm2, import `istudy.itermkeymap` under **Settings → Profiles → Keys → Key Bindings → Presets…**.
