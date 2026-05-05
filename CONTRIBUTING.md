# Contributing to Who's That Pokémon?

Thanks for taking the time to contribute! 🎮

Since the entire game lives in a single `index.html`, keeping things organised is especially important. Here's how to do it well.

---

## 🐛 Reporting Bugs

Open an [issue](../../issues) and include:

- What you expected to happen
- What actually happened
- Browser and OS (e.g. Chrome 124 on macOS 14)
- The Pokémon that caused the issue, if relevant

---

## 💡 Suggesting Features

Open an issue with the `enhancement` label. Good suggestions include:

- New hint types (describe what data they'd show and a suggested point cost)
- Scoring adjustments with reasoning
- Accessibility improvements
- UI/UX ideas

---

## 🛠️ Making Changes

### Setup

```bash
git clone https://github.com/your-username/whos-that-pokemon.git
cd whos-that-pokemon
# No install step needed — open index.html directly or:
npx serve .
```

### Code Style

The project is intentionally a single-file app. Please keep it that way. When editing:

- Keep JavaScript at the bottom inside `<script>` tags
- Keep CSS inside the `<style>` block in `<head>`
- Use `const` / `let`, not `var`
- Keep function names descriptive (`getHintHTML`, not `gh`)
- Test in at least Chrome + Firefox before opening a PR

### Adding a New Hint

1. Add an entry to the `HINTS` array with `id`, `label`, `cost`, and `icon`
2. Add a `case 'your_hint_id':` block inside `getHintHTML()`
3. Make sure the hint cost is balanced relative to how revealing it is
4. Update the hints table in `README.md`

### Pull Request Process

1. Fork → branch → commit → PR
2. PR title should be short and descriptive: `Add move-type hint` or `Fix cry button on mobile`
3. Describe what you changed and why
4. One feature / fix per PR — keep them small and focused

---

## ⚖️ Ground Rules

- Be respectful and constructive
- This is a fan project — keep all content appropriate and in the spirit of Pokémon
- Don't add external libraries without discussion (we like the zero-dependency approach)
