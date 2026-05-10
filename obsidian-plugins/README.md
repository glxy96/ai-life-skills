# Obsidian plugins

Two optional obsidian plugins that may be useful for an automated LLM second brain setup. 

## unread-dot

Shows a blue dot next to any note that has `unread: true` in its frontmatter, and auto-clears it when you open the file. Folders containing unread notes also get a dot, so you can see at a glance where new stuff lives. The `summarize` and `summarize-call` skills set `unread: true` on the notes they create, so this plugin is the visual signal that something new is waiting for you.

Bonus features:
- **"Mark all as read"** in the right-click menu on any folder.
- **"Copy callout to clipboard"** command — copies the callout under your cursor, prefixed with "Expand on this:", so you can paste it straight into a Claude conversation.

### Install

```bash
cp -r obsidian-plugins/unread-dot /path/to/your/vault/.obsidian/plugins/
```

Then in Obsidian: Settings → Community plugins → enable "Unread Dot". (You may need to toggle "Restricted mode" off first.)

## flashcards-obsidian (Anki)

Creates Anki cards from `==highlighted==` text, `Question::Answer` syntax, `#card` tags, and more. Fork of [reuseman/flashcards-obsidian](https://github.com/reuseman/flashcards-obsidian) — see [`flashcards-obsidian/README.md`](./flashcards-obsidian) here for install + Anki-Connect setup, or the [upstream wiki](https://github.com/reuseman/flashcards-obsidian/wiki) for full syntax docs.

### Install

```bash
cp -r obsidian-plugins/flashcards-obsidian /path/to/your/vault/.obsidian/plugins/
```

Then install Anki + AnkiConnect, enable the plugin in Obsidian, and configure deck/note-type in the plugin's settings.
