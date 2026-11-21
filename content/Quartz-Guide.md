---
title: Quartz & Obsidian Workflow
---

# Publishing Workflow with Quartz

You can author notes directly in Obsidian or edit Markdown files under the `content/` directory.

### 1. Creating a New Note
- Place `.md` files in the `content/` folder (or organize them into subfolders).
- Include standard frontmatter at the top:
  ```markdown
  ---
  title: Note Title
  ---
  ```

### 2. Linking Between Notes
- Use wikilinks `[[Target Note]]` or `[[Target Note|Display Name]]`. Quartz automatically parses these into navigable web links and renders preview cards.

### 3. Synchronizing Changes
Commit and push updates to your GitHub repository:
```bash
git add .
git commit -m "Add new note"
git push
```
Cloudflare Pages triggers an automated build upon every push, publishing changes globally within 1–2 minutes.

Return to: [[index|Home]]
