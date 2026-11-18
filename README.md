# VS Code Configuration

A small, personal collection of VS Code settings and JavaScript/React snippets.

## Files

| File | Purpose |
| --- | --- |
| `settings.json` | Editor, workspace, language, and extension preferences |
| `code-snippets.json` | Global snippets for JavaScript and React/JSX/TSX |

## Installation

1. Open the VS Code user configuration folder:
   - **Linux:** `~/.config/Code/User`
   - **macOS:** `~/Library/Application Support/Code/User`
   - **Windows:** `%APPDATA%\Code\User`
2. Back up the existing `settings.json` and `code-snippets.json`, if present.
3. Copy this repository's files into the user configuration folder.

> VS Code user snippets are normally stored in `~/.config/Code/User/snippets/`. If `code-snippets.json` is copied to that directory, rename it to `global.code-snippets.json`.

Restart VS Code or run **Developer: Reload Window** after copying the files.

## Settings overview

### Appearance and layout

- Uses the custom window title bar.
- Disables workbench animations and the welcome/startup editor.
- Hides the command center and workbench layout controls.
- Keeps explorer folders expanded instead of compacting nested folders.
- Uses the Material Icon Theme.

### Editing

- Automatically saves files after a short delay.
- Wraps long lines on.
- Formats files on save.
- Enables top-ranked snippets and tab-completion of snippets.
- Enables Emmet suggestions in JavaScript React and TypeScript React files.
- Associates `.js` and `.jsx` files with their React-aware language modes.

### JavaScript and TypeScript

- Disables JavaScript/TypeScript suggestions.
- Updates imports automatically when files or folders are moved.
- Shows property declaration types as inlay hints.
- Disables delete confirmation in Explorer.

### Remote development

- Configures port `3010` to use the HTTPS protocol.

## Snippet reference

Snippets are available in `.js`, `.jsx`, `.ts`, and `.tsx` files.

| Prefix | Description |
| --- | --- |
| `edf` | Export a default function component named after the current file |
| `us` | Create a `useState` declaration |
| `ue` | Create a `useEffect` block |
| `ur` | Create a `useRef` declaration |
| `range` | Create an array containing values from `1` through `N` |
| `range0` | Create an array containing values from `0` through `N - 1` |
| `map` | Render an array with `.map()` |
| `fetch` | Fetch data and manage loading state with `useEffect` |
| `cond` | Render content conditionally with `&&` |
| `onclick` | Insert an `onClick` arrow-function handler |
| `cln` | Insert a `className` attribute |
| `fmd` | Insert a Framer Motion element (`div`, `span`, `button`, `img`, or `a`) |
| `fmw` | Insert an `AnimatePresence` wrapper (`wait`, `popLayout`, or `sync`) |

Type a prefix and press **Tab** or select the suggestion to expand it.

## Customizing

Edit `settings.json` for editor and language preferences. Use the VS Code command **Preferences: Open User Settings (JSON)** to merge changes interactively.

Manage snippets with **Snippets: Configure Snippets** or **Preferences: Configure User Snippets**. A global snippet file can be shared across all projects and language scopes.

## License

Add a license if you intend to distribute this configuration publicly.
