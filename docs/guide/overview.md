# Guide Overview

This page demonstrates the key formatting features available in this docs setup.

## Callouts

This site uses [`mkdocs-callouts`](https://github.com/sondregronas/mkdocs-callouts) which lets you write callouts in **Obsidian syntax** and have them render as styled admonitions.

**Syntax:**

```markdown
> [!NOTE] Optional title
> Your content here.
```

**All supported types:**

> [!NOTE] Note
> Use this for general information that is worth highlighting.

> [!TIP] Tip
> A helpful suggestion that makes things easier.

> [!WARNING] Warning
> Something the reader should be careful about.

> [!DANGER] Danger
> A critical issue that could cause data loss or breakage.

> [!INFO] Info
> Background context or neutral supplementary information.

> [!SUCCESS] Success
> Confirmation that something worked or a recommended approach.

**Foldable callouts** — add `-` to collapse by default, `+` to expand:

> [!INFO]- Click to expand
> This callout is **collapsed by default**. The reader can open it manually.

---

## Text formatting

You can use standard Markdown formatting throughout:

- **Bold text** for emphasis
- *Italic* for lighter emphasis
- `inline code` for commands or values
- ~~Strikethrough~~ for deprecated content
- ==Highlighted== text (requires `pymdownx.mark`)

A **well-structured paragraph** breaks ideas into short, scannable chunks. Keep sentences direct. Avoid padding.

---

## Images

Images go in `docs/assets/` and are referenced with a relative path:

```markdown
![Alt text](../assets/example.svg)
```

![Example image](../assets/example.svg)
