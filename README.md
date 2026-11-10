# Obsidian Configuration

A reusable Obsidian vault configuration with a Vim-oriented editor, the AnuPpuccin theme, a set of community plugins, and a prepared sidebar layout. The repository contains configuration and bundled plugin and theme files; it does not include notes, templates, or drawings.

## Setup

1. Close Obsidian and copy the `.obsidian` directory into the root of a vault. Back up any existing `.obsidian` directory first, since copying it over can replace that vault's settings and workspace.
2. Open the vault in Obsidian. Enable community plugins if prompted, and review the installed plugins and their settings before use.
3. Create or select folders for attachments (`attachments`), daily notes (`todos`), and templates (`templates`), or change those paths in Obsidian settings. Excalidraw uses `Excalidraw` for drawings and has configured paths beneath it for templates, scripts, and fonts.
4. Configure Git and any remote separately if using Git integration. Choose an export destination and site name in Webpage HTML Export before exporting.

The saved workspace opens with an empty main pane. Files, Search, and Bookmarks occupy the left sidebar; Outgoing links, Tags, Outline, Calendar, Backlinks, and All properties share the upper right tab group, with Source Control in a separate group below. Both sidebars are 300 pixels wide. Obsidian may update `workspace.json` as the workspace changes.

## Configuration

- Vim mode and automatic link updates are enabled; attachments are saved to `attachments`.
- Daily notes use `todos`; the core Templates plugin uses `templates`.
- AnuPpuccin is selected, with Style Settings configured for a card layout, floating status bar and header, and rosewater accent. Two CSS snippets are included (`catppuccin-text-highlights` and `custom-rainbow-colors`); enable them in Appearance if desired.
- Git is configured for automatic commits every 30 minutes and pulls every 90 minutes, with no automatic push interval. Review these settings for the target vault and remote.
- Custom shortcuts use `Mod` (Command on macOS, Control on Windows/Linux): `Mod+Shift+K` opens Calendar, `Mod+Shift+X` inserts a math block, and `Mod+Shift+E` / `Mod+Shift+Q` create Excalidraw drawings. The delete-paragraph shortcut is cleared.
- Core plugins enabled: File explorer, Search, Quick switcher, Graph view, Backlinks, Canvas, Outgoing links, Tags view, Properties view, Page preview, Daily notes, Templates, Note composer, Command palette, Editor status, Bookmarks, Outline, Word count, File recovery, Sync, and Bases. Sync still requires a separately configured Obsidian Sync account and remote vault.

## Included packages

All nine listed community plugins are enabled in `community-plugins.json`. Versions are those bundled in this repository, not necessarily the latest releases.

| Package | Version | Purpose |
| --- | --- | --- |
| Calendar | 1.5.10 | Calendar view for daily notes. |
| Excalidraw | 2.18.2 | Create and edit drawings in the vault. |
| Git | 2.35.2 | Version control, backups, and source control. |
| Iconize | 2.14.7 | Add icons to files, folders, and text. |
| Linter | 1.30.0 | Format and standardize Markdown notes. |
| PDF++ | 0.40.31 | Annotate PDFs and link to selections. |
| Style Settings | 1.0.9 | Adjust theme, plugin, and snippet styling. |
| Table Extended | 1.6.1 | Extended tables using MultiMarkdown syntax. |
| Webpage HTML Export | 1.9.2 | Export notes, canvases, or vaults to HTML; desktop only. |
| AnuPpuccin theme | 1.5.0 | Catppuccin-inspired theme and layout options. |

Plugin and theme settings live under `.obsidian/plugins` and `.obsidian/themes`; core settings, shortcuts, and workspace state live directly under `.obsidian`. Update bundled packages through Obsidian as needed, and review compatibility with the Obsidian version in use.
